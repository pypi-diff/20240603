# Comparing `tmp/qt4a-2.3.1.tar.gz` & `tmp/qt4a-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qt4a-2.3.1.tar", last modified: Wed Apr 28 01:23:58 2021, max compression
+gzip compressed data, was "qt4a-3.0.0.tar", last modified: Mon Jun  3 13:12:15 2024, max compression
```

## Comparing `qt4a-2.3.1.tar` & `qt4a-3.0.0.tar`

### file list

```diff
@@ -1,107 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-28 01:23:58.872004 qt4a-2.3.1/
--rw-r--r--   0 runner    (1001) docker     (121)       69 2021-04-28 01:23:49.000000 qt4a-2.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3097 2021-04-28 01:23:58.872004 qt4a-2.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2233 2021-04-28 01:23:49.000000 qt4a-2.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-28 01:23:58.848004 qt4a-2.3.1/qt4a/
--rw-r--r--   0 runner    (1001) docker     (121)      762 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      851 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    81712 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/andrcontrols.py
--rw-r--r--   0 runner    (1001) docker     (121)    16689 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/androidapp.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-28 01:23:58.848004 qt4a-2.3.1/qt4a/androiddriver/
--rw-r--r--   0 runner    (1001) docker     (121)      748 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/androiddriver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17826 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/androiddriver/_axmlparser.py
--rw-r--r--   0 runner    (1001) docker     (121)    74579 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/androiddriver/adb.py
--rw-r--r--   0 runner    (1001) docker     (121)    22289 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/androiddriver/adbclient.py
--rw-r--r--   0 runner    (1001) docker     (121)    41580 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/androiddriver/androiddriver.py
--rw-r--r--   0 runner    (1001) docker     (121)     7574 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/androiddriver/clientsocket.py
--rw-r--r--   0 runner    (1001) docker     (121)    40656 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/androiddriver/devicedriver.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-28 01:23:58.852004 qt4a-2.3.1/qt4a/androiddriver/tools/
--rw-r--r--   0 runner    (1001) docker     (121)    53656 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/androiddriver/tools/AndroidSpy.jar
--rw-r--r--   0 runner    (1001) docker     (121)   374996 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/androiddriver/tools/QT4AHelper.apk
--rw-r--r--   0 runner    (1001) docker     (121)    58406 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/androiddriver/tools/SpyHelper.jar
--rw-r--r--   0 runner    (1001) docker     (121)     2834 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/androiddriver/tools/SpyHelper.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-28 01:23:58.844004 qt4a-2.3.1/qt4a/androiddriver/tools/adb/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-28 01:23:58.852004 qt4a-2.3.1/qt4a/androiddriver/tools/adb/darwin/
--rw-r--r--   0 runner    (1001) docker     (121)  2622660 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/androiddriver/tools/adb/darwin/adb
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-28 01:23:58.852004 qt4a-2.3.1/qt4a/androiddriver/tools/adb/linux2/
--rw-r--r--   0 runner    (1001) docker     (121)  2704537 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/androiddriver/tools/adb/linux2/adb
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-28 01:23:58.856004 qt4a-2.3.1/qt4a/androiddriver/tools/adb/win32/
--rw-r--r--   0 runner    (1001) docker     (121)    97792 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/androiddriver/tools/adb/win32/AdbWinApi.dll
--rw-r--r--   0 runner    (1001) docker     (121)    62976 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/androiddriver/tools/adb/win32/AdbWinUsbApi.dll
--rw-r--r--   0 runner    (1001) docker     (121)  1868800 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/androiddriver/tools/adb/win32/adb.exe
--rw-r--r--   0 runner    (1001) docker     (121)     5164 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/androiddriver/tools/androidhook.jar
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-28 01:23:58.860004 qt4a-2.3.1/qt4a/androiddriver/tools/arm64-v8a/
--rwxr-xr-x   0 runner    (1001) docker     (121)    18528 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/androiddriver/tools/arm64-v8a/droid_inject
--rwxr-xr-x   0 runner    (1001) docker     (121)    23032 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/androiddriver/tools/arm64-v8a/droid_inject64
--rw-r--r--   0 runner    (1001) docker     (121)    33932 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/androiddriver/tools/arm64-v8a/libandroidhook.so
--rw-r--r--   0 runner    (1001) docker     (121)    87420 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/androiddriver/tools/arm64-v8a/libandroidhook_art.so
--rw-r--r--   0 runner    (1001) docker     (121)    17556 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/androiddriver/tools/arm64-v8a/libdexloader.so
--rw-r--r--   0 runner    (1001) docker     (121)    13704 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/androiddriver/tools/arm64-v8a/libdexloader64.so
--rw-r--r--   0 runner    (1001) docker     (121)   362204 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/androiddriver/tools/arm64-v8a/screenkit
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-28 01:23:58.860004 qt4a-2.3.1/qt4a/androiddriver/tools/armeabi/
--rwxr-xr-x   0 runner    (1001) docker     (121)    18528 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/androiddriver/tools/armeabi/droid_inject
--rw-r--r--   0 runner    (1001) docker     (121)    33924 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/androiddriver/tools/armeabi/libandroidhook.so
--rw-r--r--   0 runner    (1001) docker     (121)    91516 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/androiddriver/tools/armeabi/libandroidhook_art.so
--rw-r--r--   0 runner    (1001) docker     (121)    17548 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/androiddriver/tools/armeabi/libdexloader.so
--rw-r--r--   0 runner    (1001) docker     (121)   362204 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/androiddriver/tools/armeabi/screenkit
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-28 01:23:58.864004 qt4a-2.3.1/qt4a/androiddriver/tools/armeabi-v7a/
--rwxr-xr-x   0 runner    (1001) docker     (121)    18536 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/androiddriver/tools/armeabi-v7a/droid_inject
--rw-r--r--   0 runner    (1001) docker     (121)    33932 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/androiddriver/tools/armeabi-v7a/libandroidhook.so
--rw-r--r--   0 runner    (1001) docker     (121)    87420 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/androiddriver/tools/armeabi-v7a/libandroidhook_art.so
--rw-r--r--   0 runner    (1001) docker     (121)    17556 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/androiddriver/tools/armeabi-v7a/libdexloader.so
--rw-r--r--   0 runner    (1001) docker     (121)   362204 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/androiddriver/tools/armeabi-v7a/screenkit
--rw-r--r--   0 runner    (1001) docker     (121)      335 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/androiddriver/tools/inject
--rw-r--r--   0 runner    (1001) docker     (121)      341 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/androiddriver/tools/inject64
--rw-r--r--   0 runner    (1001) docker     (121)        3 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/androiddriver/tools/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-28 01:23:58.864004 qt4a-2.3.1/qt4a/androiddriver/tools/x86/
--rwxr-xr-x   0 runner    (1001) docker     (121)    18508 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/androiddriver/tools/x86/droid_inject
--rw-r--r--   0 runner    (1001) docker     (121)    17632 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/androiddriver/tools/x86/libandroidhook.so
--rw-r--r--   0 runner    (1001) docker     (121)   136436 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/androiddriver/tools/x86/libandroidhook_art.so
--rw-r--r--   0 runner    (1001) docker     (121)    13356 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/androiddriver/tools/x86/libdexloader.so
--rw-r--r--   0 runner    (1001) docker     (121)   739024 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/androiddriver/tools/x86/screenkit
--rw-r--r--   0 runner    (1001) docker     (121)    21196 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/androiddriver/util.py
--rw-r--r--   0 runner    (1001) docker     (121)    67849 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/androiddriver/webdriver.py
--rw-r--r--   0 runner    (1001) docker     (121)    18464 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/androidtestbase.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-28 01:23:58.864004 qt4a-2.3.1/qt4a/apktool/
--rw-r--r--   0 runner    (1001) docker     (121)      811 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/apktool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3798 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/apktool/apkfile.py
--rw-r--r--   0 runner    (1001) docker     (121)    34506 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/apktool/axml.py
--rw-r--r--   0 runner    (1001) docker     (121)     5813 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/apktool/header.py
--rw-r--r--   0 runner    (1001) docker     (121)     6051 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/apktool/manifest.py
--rw-r--r--   0 runner    (1001) docker     (121)    11588 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/apktool/repack.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-28 01:23:58.868004 qt4a-2.3.1/qt4a/apktool/tools/
--rw-r--r--   0 runner    (1001) docker     (121)   829114 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/apktool/tools/apkhelper.jar
--rw-r--r--   0 runner    (1001) docker     (121)   378662 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/apktool/tools/asm-debug-all-5.0.3.jar
--rw-r--r--   0 runner    (1001) docker     (121)    17746 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/apktool/tools/d2j-base-cmd-2.1-SNAPSHOT.jar
--rw-r--r--   0 runner    (1001) docker     (121)   236417 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/apktool/tools/dex-ir-2.1-SNAPSHOT.jar
--rw-r--r--   0 runner    (1001) docker     (121)    72014 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/apktool/tools/dex-reader-2.1-SNAPSHOT.jar
--rw-r--r--   0 runner    (1001) docker     (121)    79198 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/apktool/tools/dex-reader-api-2.1-SNAPSHOT.jar
--rw-r--r--   0 runner    (1001) docker     (121)   174385 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/apktool/tools/dex-tools-2.1-SNAPSHOT.jar
--rw-r--r--   0 runner    (1001) docker     (121)   108357 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/apktool/tools/dex-translator-2.1-SNAPSHOT.jar
--rw-r--r--   0 runner    (1001) docker     (121)    26764 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/apktool/tools/dexloader.dex
--rw-r--r--   0 runner    (1001) docker     (121)   962823 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/apktool/tools/dx.jar
--rw-r--r--   0 runner    (1001) docker     (121)     2233 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/apktool/tools/qt4a.keystore
--rw-r--r--   0 runner    (1001) docker     (121)     4075 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/browser.py
--rw-r--r--   0 runner    (1001) docker     (121)    48036 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/device.py
--rw-r--r--   0 runner    (1001) docker     (121)     7618 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/management.py
--rw-r--r--   0 runner    (1001) docker     (121)     5304 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/mtcontrols.py
--rw-r--r--   0 runner    (1001) docker     (121)     1630 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/qpath.py
--rw-r--r--   0 runner    (1001) docker     (121)     5314 2021-04-28 01:23:49.000000 qt4a-2.3.1/qt4a/systemui.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-28 01:23:58.848004 qt4a-2.3.1/qt4a.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3097 2021-04-28 01:23:58.000000 qt4a-2.3.1/qt4a.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3065 2021-04-28 01:23:58.000000 qt4a-2.3.1/qt4a.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-28 01:23:58.000000 qt4a-2.3.1/qt4a.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       66 2021-04-28 01:23:58.000000 qt4a-2.3.1/qt4a.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-28 01:23:58.000000 qt4a-2.3.1/qt4a.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       23 2021-04-28 01:23:58.000000 qt4a-2.3.1/qt4a.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2021-04-28 01:23:58.000000 qt4a-2.3.1/qt4a.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-04-28 01:23:49.000000 qt4a-2.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-04-28 01:23:58.872004 qt4a-2.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3428 2021-04-28 01:23:49.000000 qt4a-2.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-28 01:23:58.872004 qt4a-2.3.1/test/
--rw-r--r--   0 runner    (1001) docker     (121)     1846 2021-04-28 01:23:49.000000 qt4a-2.3.1/test/test_andrcontrols.py
--rw-r--r--   0 runner    (1001) docker     (121)     3395 2021-04-28 01:23:49.000000 qt4a-2.3.1/test/test_androidapp.py
--rw-r--r--   0 runner    (1001) docker     (121)     5458 2021-04-28 01:23:49.000000 qt4a-2.3.1/test/test_device.py
--rw-r--r--   0 runner    (1001) docker     (121)     2120 2021-04-28 01:23:49.000000 qt4a-2.3.1/test/test_management.py
--rw-r--r--   0 runner    (1001) docker     (121)     1849 2021-04-28 01:23:49.000000 qt4a-2.3.1/test/test_qpath.py
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-04-28 01:23:58.000000 qt4a-2.3.1/version.txt
+drwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)        0 2024-06-03 13:12:15.796255 qt4a-3.0.0/
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)       69 2024-06-03 11:01:47.000000 qt4a-3.0.0/MANIFEST.in
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)     3223 2024-06-03 13:12:15.796255 qt4a-3.0.0/PKG-INFO
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)     2359 2024-06-03 11:01:47.000000 qt4a-3.0.0/README.md
+drwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)        0 2024-06-03 13:12:15.620916 qt4a-3.0.0/qt4a/
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)      762 2020-10-05 18:06:54.000000 qt4a-3.0.0/qt4a/__init__.py
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)      851 2020-10-05 18:06:54.000000 qt4a-3.0.0/qt4a/__main__.py
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)    84369 2024-04-26 11:52:18.000000 qt4a-3.0.0/qt4a/andrcontrols.py
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)    18094 2024-06-03 11:01:02.000000 qt4a-3.0.0/qt4a/androidapp.py
+drwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)        0 2024-06-03 13:12:15.646630 qt4a-3.0.0/qt4a/androiddriver/
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)      748 2020-10-05 18:06:54.000000 qt4a-3.0.0/qt4a/androiddriver/__init__.py
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)    17826 2020-10-05 18:06:54.000000 qt4a-3.0.0/qt4a/androiddriver/_axmlparser.py
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)    75232 2024-06-03 11:01:02.000000 qt4a-3.0.0/qt4a/androiddriver/adb.py
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)    22289 2021-01-07 12:19:58.000000 qt4a-3.0.0/qt4a/androiddriver/adbclient.py
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)    41544 2024-04-26 11:52:18.000000 qt4a-3.0.0/qt4a/androiddriver/androiddriver.py
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)     7574 2023-02-08 03:30:30.000000 qt4a-3.0.0/qt4a/androiddriver/clientsocket.py
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)    41891 2024-04-26 11:52:18.000000 qt4a-3.0.0/qt4a/androiddriver/devicedriver.py
+drwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)        0 2024-06-03 13:12:15.662365 qt4a-3.0.0/qt4a/androiddriver/tools/
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)    79430 2024-04-26 11:52:18.000000 qt4a-3.0.0/qt4a/androiddriver/tools/AndroidSpy.jar
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)   296564 2022-07-22 07:28:34.000000 qt4a-3.0.0/qt4a/androiddriver/tools/QT4AHelper.apk
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)    59421 2023-11-21 01:35:06.000000 qt4a-3.0.0/qt4a/androiddriver/tools/SpyHelper.jar
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)     2834 2020-10-05 18:06:54.000000 qt4a-3.0.0/qt4a/androiddriver/tools/SpyHelper.sh
+drwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)        0 2024-06-03 13:12:15.594103 qt4a-3.0.0/qt4a/androiddriver/tools/adb/
+drwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)        0 2024-06-03 13:12:15.664405 qt4a-3.0.0/qt4a/androiddriver/tools/adb/darwin/
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)  2622660 2020-10-05 18:06:55.000000 qt4a-3.0.0/qt4a/androiddriver/tools/adb/darwin/adb
+drwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)        0 2024-06-03 13:12:15.671009 qt4a-3.0.0/qt4a/androiddriver/tools/adb/linux2/
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)  2704537 2020-10-05 18:06:55.000000 qt4a-3.0.0/qt4a/androiddriver/tools/adb/linux2/adb
+drwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)        0 2024-06-03 13:12:15.681263 qt4a-3.0.0/qt4a/androiddriver/tools/adb/win32/
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)    97792 2020-10-05 18:06:55.000000 qt4a-3.0.0/qt4a/androiddriver/tools/adb/win32/AdbWinApi.dll
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)    62976 2020-10-05 18:06:55.000000 qt4a-3.0.0/qt4a/androiddriver/tools/adb/win32/AdbWinUsbApi.dll
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)  1868800 2020-10-05 18:06:55.000000 qt4a-3.0.0/qt4a/androiddriver/tools/adb/win32/adb.exe
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)     5164 2020-10-05 18:06:55.000000 qt4a-3.0.0/qt4a/androiddriver/tools/androidhook.jar
+drwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)        0 2024-06-03 13:12:15.700718 qt4a-3.0.0/qt4a/androiddriver/tools/arm64-v8a/
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)    18528 2021-04-24 02:34:24.000000 qt4a-3.0.0/qt4a/androiddriver/tools/arm64-v8a/droid_inject
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)    23032 2021-04-24 02:34:24.000000 qt4a-3.0.0/qt4a/androiddriver/tools/arm64-v8a/droid_inject64
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)   335148 2024-04-26 11:52:18.000000 qt4a-3.0.0/qt4a/androiddriver/tools/arm64-v8a/libandroidhook.so
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)   502280 2024-06-03 11:01:02.000000 qt4a-3.0.0/qt4a/androiddriver/tools/arm64-v8a/libandroidhook64.so
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)    21984 2024-04-26 11:52:18.000000 qt4a-3.0.0/qt4a/androiddriver/tools/arm64-v8a/libdexloader.so
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)    14016 2024-04-26 11:52:18.000000 qt4a-3.0.0/qt4a/androiddriver/tools/arm64-v8a/libdexloader64.so
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)   362204 2020-10-05 18:06:55.000000 qt4a-3.0.0/qt4a/androiddriver/tools/arm64-v8a/screenkit
+drwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)        0 2024-06-03 13:12:15.708696 qt4a-3.0.0/qt4a/androiddriver/tools/armeabi/
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)    18528 2021-04-24 02:34:24.000000 qt4a-3.0.0/qt4a/androiddriver/tools/armeabi/droid_inject
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)    21984 2024-04-26 11:52:18.000000 qt4a-3.0.0/qt4a/androiddriver/tools/armeabi/libdexloader.so
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)   362204 2020-10-05 18:06:55.000000 qt4a-3.0.0/qt4a/androiddriver/tools/armeabi/screenkit
+drwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)        0 2024-06-03 13:12:15.718392 qt4a-3.0.0/qt4a/androiddriver/tools/armeabi-v7a/
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)    18536 2021-04-24 02:34:24.000000 qt4a-3.0.0/qt4a/androiddriver/tools/armeabi-v7a/droid_inject
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)   335148 2024-04-26 11:52:18.000000 qt4a-3.0.0/qt4a/androiddriver/tools/armeabi-v7a/libandroidhook.so
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)    21984 2024-04-26 11:52:18.000000 qt4a-3.0.0/qt4a/androiddriver/tools/armeabi-v7a/libdexloader.so
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)   362204 2020-10-05 18:06:55.000000 qt4a-3.0.0/qt4a/androiddriver/tools/armeabi-v7a/screenkit
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)      335 2020-10-05 18:06:55.000000 qt4a-3.0.0/qt4a/androiddriver/tools/inject
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)      341 2020-10-05 18:06:55.000000 qt4a-3.0.0/qt4a/androiddriver/tools/inject64
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)        4 2024-06-03 11:01:02.000000 qt4a-3.0.0/qt4a/androiddriver/tools/version.txt
+drwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)        0 2024-06-03 13:12:15.727106 qt4a-3.0.0/qt4a/androiddriver/tools/x86/
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)    18508 2021-04-24 02:34:24.000000 qt4a-3.0.0/qt4a/androiddriver/tools/x86/droid_inject
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)   493308 2024-04-26 11:52:18.000000 qt4a-3.0.0/qt4a/androiddriver/tools/x86/libandroidhook.so
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)    13728 2024-04-26 11:52:18.000000 qt4a-3.0.0/qt4a/androiddriver/tools/x86/libdexloader.so
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)   739024 2020-10-05 18:06:55.000000 qt4a-3.0.0/qt4a/androiddriver/tools/x86/screenkit
+drwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)        0 2024-06-03 13:12:15.746311 qt4a-3.0.0/qt4a/androiddriver/tools/x86_64/
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)    18508 2022-05-16 14:56:58.000000 qt4a-3.0.0/qt4a/androiddriver/tools/x86_64/droid_inject
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)    23464 2024-04-26 11:52:18.000000 qt4a-3.0.0/qt4a/androiddriver/tools/x86_64/droid_inject64
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)   493308 2024-04-26 11:52:18.000000 qt4a-3.0.0/qt4a/androiddriver/tools/x86_64/libandroidhook.so
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)   524232 2024-04-26 11:52:18.000000 qt4a-3.0.0/qt4a/androiddriver/tools/x86_64/libandroidhook64.so
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)    13728 2024-04-26 11:52:18.000000 qt4a-3.0.0/qt4a/androiddriver/tools/x86_64/libdexloader.so
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)    14360 2024-04-26 11:52:18.000000 qt4a-3.0.0/qt4a/androiddriver/tools/x86_64/libdexloader64.so
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)   739024 2022-05-16 14:56:58.000000 qt4a-3.0.0/qt4a/androiddriver/tools/x86_64/screenkit
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)    21956 2024-06-03 11:05:52.000000 qt4a-3.0.0/qt4a/androiddriver/util.py
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)    67849 2020-10-05 18:06:55.000000 qt4a-3.0.0/qt4a/androiddriver/webdriver.py
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)    19668 2023-02-08 03:30:30.000000 qt4a-3.0.0/qt4a/androidtestbase.py
+drwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)        0 2024-06-03 13:12:15.758520 qt4a-3.0.0/qt4a/apktool/
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)      811 2020-10-05 18:06:55.000000 qt4a-3.0.0/qt4a/apktool/__init__.py
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)     3798 2020-10-05 18:06:55.000000 qt4a-3.0.0/qt4a/apktool/apkfile.py
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)    34644 2024-06-03 11:01:14.000000 qt4a-3.0.0/qt4a/apktool/axml.py
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)     5813 2020-10-05 18:06:55.000000 qt4a-3.0.0/qt4a/apktool/header.py
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)     6051 2020-10-05 18:06:55.000000 qt4a-3.0.0/qt4a/apktool/manifest.py
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)    12254 2024-06-03 11:01:14.000000 qt4a-3.0.0/qt4a/apktool/repack.py
+drwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)        0 2024-06-03 13:12:15.786337 qt4a-3.0.0/qt4a/apktool/tools/
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)   829114 2020-10-05 18:06:55.000000 qt4a-3.0.0/qt4a/apktool/tools/apkhelper.jar
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)   378662 2020-10-05 18:06:55.000000 qt4a-3.0.0/qt4a/apktool/tools/asm-debug-all-5.0.3.jar
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)    17746 2020-10-05 18:06:55.000000 qt4a-3.0.0/qt4a/apktool/tools/d2j-base-cmd-2.1-SNAPSHOT.jar
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)   236417 2020-10-05 18:06:55.000000 qt4a-3.0.0/qt4a/apktool/tools/dex-ir-2.1-SNAPSHOT.jar
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)    72014 2020-10-05 18:06:55.000000 qt4a-3.0.0/qt4a/apktool/tools/dex-reader-2.1-SNAPSHOT.jar
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)    79198 2020-10-05 18:06:55.000000 qt4a-3.0.0/qt4a/apktool/tools/dex-reader-api-2.1-SNAPSHOT.jar
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)   174385 2020-10-05 18:06:55.000000 qt4a-3.0.0/qt4a/apktool/tools/dex-tools-2.1-SNAPSHOT.jar
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)   108357 2020-10-05 18:06:55.000000 qt4a-3.0.0/qt4a/apktool/tools/dex-translator-2.1-SNAPSHOT.jar
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)    29584 2024-04-26 11:52:18.000000 qt4a-3.0.0/qt4a/apktool/tools/dexloader.dex
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)   962823 2020-10-05 18:06:55.000000 qt4a-3.0.0/qt4a/apktool/tools/dx.jar
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)     2233 2020-10-05 18:06:55.000000 qt4a-3.0.0/qt4a/apktool/tools/qt4a.keystore
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)     4075 2020-10-05 18:06:55.000000 qt4a-3.0.0/qt4a/browser.py
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)    50347 2024-05-27 11:39:50.000000 qt4a-3.0.0/qt4a/device.py
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)     8690 2024-04-26 11:52:18.000000 qt4a-3.0.0/qt4a/management.py
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)     5304 2020-10-05 18:06:55.000000 qt4a-3.0.0/qt4a/mtcontrols.py
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)     1630 2020-10-05 18:06:55.000000 qt4a-3.0.0/qt4a/qpath.py
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)     5314 2020-10-05 18:06:55.000000 qt4a-3.0.0/qt4a/systemui.py
+drwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)        0 2024-06-03 13:12:15.631646 qt4a-3.0.0/qt4a.egg-info/
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)     3223 2024-06-03 13:12:15.000000 qt4a-3.0.0/qt4a.egg-info/PKG-INFO
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)     3181 2024-06-03 13:12:15.000000 qt4a-3.0.0/qt4a.egg-info/SOURCES.txt
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)        1 2024-06-03 13:12:15.000000 qt4a-3.0.0/qt4a.egg-info/dependency_links.txt
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)       66 2024-06-03 13:12:15.000000 qt4a-3.0.0/qt4a.egg-info/entry_points.txt
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)        1 2024-06-03 13:12:15.000000 qt4a-3.0.0/qt4a.egg-info/not-zip-safe
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)       23 2024-06-03 13:12:15.000000 qt4a-3.0.0/qt4a.egg-info/requires.txt
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)        5 2024-06-03 13:12:15.000000 qt4a-3.0.0/qt4a.egg-info/top_level.txt
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)       22 2024-06-03 11:01:47.000000 qt4a-3.0.0/requirements.txt
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)       38 2024-06-03 13:12:15.797252 qt4a-3.0.0/setup.cfg
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)     3428 2024-06-03 11:01:47.000000 qt4a-3.0.0/setup.py
+drwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)        0 2024-06-03 13:12:15.794259 qt4a-3.0.0/test/
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)     1846 2020-10-05 18:06:55.000000 qt4a-3.0.0/test/test_andrcontrols.py
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)     3395 2020-10-05 18:06:55.000000 qt4a-3.0.0/test/test_androidapp.py
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)     5463 2024-04-27 00:10:34.000000 qt4a-3.0.0/test/test_device.py
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)     2120 2020-10-05 18:06:55.000000 qt4a-3.0.0/test/test_management.py
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)     1849 2020-10-05 18:06:55.000000 qt4a-3.0.0/test/test_qpath.py
+-rwxrwxrwx   0 shadowyang  (1000) shadowyang  (1000)        6 2024-06-03 13:12:08.000000 qt4a-3.0.0/version.txt
```

### Comparing `qt4a-2.3.1/PKG-INFO` & `qt4a-3.0.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: qt4a
-Version: 2.3.1
+Version: 3.0.0
 Summary: QTA driver for Android app
 Home-page: https://github.com/Tencent/QT4A
 Author: Tencent
 License: Copyright(c)2010-2018 Tencent All Rights Reserved. 
 Project-URL: QT4A Documentation, https://qt4a.readthedocs.io/zh_CN/latest/
 Description: # QT4A
         
-        [![Build Status](https://travis-ci.org/Tencent/QT4A.svg?branch=master)](https://travis-ci.org/Tencent/QT4A) 
+        [![Build Status](https://github.com/tencent/qt4a/actions/workflows/unittest.yml/badge.svg)](https://github.com/Tencent/QT4A/actions/workflows/unittest.yml) 
         [![PyPi version](https://img.shields.io/pypi/v/qt4a.svg)](https://pypi.python.org/pypi/qt4a/) 
         [![Documentation Status](https://readthedocs.org/projects/qt4a/badge/?version=latest)](https://qt4a.readthedocs.io/zh_CN/latest/?badge=latest)
         [![GitHub tag](https://img.shields.io/github/tag/Tencent/QT4A.svg)](https://GitHub.com/Tencent/QT4A/tags/)
         [![codecov.io](https://codecov.io/github/tencent/QT4A/coverage.svg?branch=master)](https://codecov.io/github/tencent/QT4A)
         
         QT4A (Quick Test for Android) is a QTA test automation driver for Android application.
         
         ### Features
         
-         * Support most versions of Android OS from 2.3 to 8.1 
+         * Support most versions of Android OS from 4.0 to 14(armeabi-v7a、arm64-v8a、x86、x86_64)
          * Multiple devices can be used simultaneously in a test
          * Support testing multi-process application, and multiple application can be tested simultaneously
          * Support testting code obfuscated application
          * Support testing with custom controls
          * Support non-root devices
          
         QT4A should be used with [QTAF](https://github.com/Tencent/QTAF), please check it first.
@@ -35,15 +35,15 @@
         
         ------------------------------
         
         QT4A (Quick Test for Android)，基于QTA提供面向Android应用的UI测试自动化测试解决方案。
         
         ### 特性介绍
         
-        1. 支持Android 2.3 - 8.1版本
+        1. 支持Android 4.0 - 14 版本(armeabi-v7a、arm64-v8a、x86、x86_64)
         2. 支持多设备协同测试
         3. 支持跨进程、跨应用测试
         4. 支持进行过控件混淆的安装包
         5. 支持自定义（自绘）控件
         6. 支持非root设备
         
         QT4A需要和[QTAF](https://github.com/Tencent/QTAF)一起使用，请先参考QTAF的使用
```

### Comparing `qt4a-2.3.1/README.md` & `qt4a-3.0.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # QT4A
 
-[![Build Status](https://travis-ci.org/Tencent/QT4A.svg?branch=master)](https://travis-ci.org/Tencent/QT4A) 
+[![Build Status](https://github.com/tencent/qt4a/actions/workflows/unittest.yml/badge.svg)](https://github.com/Tencent/QT4A/actions/workflows/unittest.yml) 
 [![PyPi version](https://img.shields.io/pypi/v/qt4a.svg)](https://pypi.python.org/pypi/qt4a/) 
 [![Documentation Status](https://readthedocs.org/projects/qt4a/badge/?version=latest)](https://qt4a.readthedocs.io/zh_CN/latest/?badge=latest)
 [![GitHub tag](https://img.shields.io/github/tag/Tencent/QT4A.svg)](https://GitHub.com/Tencent/QT4A/tags/)
 [![codecov.io](https://codecov.io/github/tencent/QT4A/coverage.svg?branch=master)](https://codecov.io/github/tencent/QT4A)
 
 QT4A (Quick Test for Android) is a QTA test automation driver for Android application.
 
 ### Features
 
- * Support most versions of Android OS from 2.3 to 8.1 
+ * Support most versions of Android OS from 4.0 to 14(armeabi-v7a、arm64-v8a、x86、x86_64)
  * Multiple devices can be used simultaneously in a test
  * Support testing multi-process application, and multiple application can be tested simultaneously
  * Support testting code obfuscated application
  * Support testing with custom controls
  * Support non-root devices
  
 QT4A should be used with [QTAF](https://github.com/Tencent/QTAF), please check it first.
@@ -27,15 +27,15 @@
 
 ------------------------------
 
 QT4A (Quick Test for Android)，基于QTA提供面向Android应用的UI测试自动化测试解决方案。
 
 ### 特性介绍
 
-1. 支持Android 2.3 - 8.1版本
+1. 支持Android 4.0 - 14 版本(armeabi-v7a、arm64-v8a、x86、x86_64)
 2. 支持多设备协同测试
 3. 支持跨进程、跨应用测试
 4. 支持进行过控件混淆的安装包
 5. 支持自定义（自绘）控件
 6. 支持非root设备
 
 QT4A需要和[QTAF](https://github.com/Tencent/QTAF)一起使用，请先参考QTAF的使用
```

### Comparing `qt4a-2.3.1/qt4a/__init__.py` & `qt4a-3.0.0/qt4a/__init__.py`

 * *Files identical despite different names*

### Comparing `qt4a-2.3.1/qt4a/__main__.py` & `qt4a-3.0.0/qt4a/__main__.py`

 * *Files identical despite different names*

### Comparing `qt4a-2.3.1/qt4a/andrcontrols.py` & `qt4a-3.0.0/qt4a/andrcontrols.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,214 +1,231 @@
 # -*- coding: UTF-8 -*-
 #
 # Tencent is pleased to support the open source community by making QTA available.
 # Copyright (C) 2016THL A29 Limited, a Tencent company. All rights reserved.
-# Licensed under the BSD 3-Clause License (the "License"); you may not use this 
+# Licensed under the BSD 3-Clause License (the "License"); you may not use this
 # file except in compliance with the License. You may obtain a copy of the License at
-# 
+#
 # https://opensource.org/licenses/BSD-3-Clause
-# 
-# Unless required by applicable law or agreed to in writing, software distributed 
+#
+# Unless required by applicable law or agreed to in writing, software distributed
 # under the License is distributed on an "AS IS" basis, WITHOUT WARRANTIES OR CONDITIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 #
 
-'''定义Android控件
-'''
+"""定义Android控件
+"""
 
 import io
 import os
 import tempfile
 import time
 
 import six
 from testbase.util import LazyInit, Timeout
 from tuia.exceptions import ControlNotFoundError
 
 from qt4a.androiddriver.androiddriver import AndroidDriver
-from qt4a.androiddriver.util import Deprecated, get_intersection, logger
+from qt4a.androiddriver.util import Deprecated, get_intersection, logger, general_encode
+
 
 def lazy_init(func):
-    '''调用到此函数时进入延迟初始化逻辑
-    '''
+    """调用到此函数时进入延迟初始化逻辑
+    """
+
     def wrap_func(self, *args, **kwds):
         self._lazy_obj._app  # 调到窗口类的延迟初始化函数
         return func(self, *args, **kwds)
+
     return wrap_func
 
+
 class Window(object):
-    '''控件容器基类
-    '''
-    Process = ''  # 所在的进程名，不填表示是主进程
-    Activity = ''  # 所在的Activity
+    """控件容器基类
+    """
+
+    Process = ""  # 所在的进程名，不填表示是主进程
+    Activity = ""  # 所在的Activity
 
     def __init__(self, app_or_driver, wait_activity=True, **kwds):
         self._locators = {}
         self._device = None
         self._app = None
-        if hasattr(app_or_driver, '_drivers'):
+        if hasattr(app_or_driver, "_drivers"):
             # AndroidApp类型
             self._driver = app_or_driver.get_driver(self.Process)
             self._device = app_or_driver.device
             self._app = app_or_driver
-        elif hasattr(app_or_driver, '_driver'):
+        elif hasattr(app_or_driver, "_driver"):
             # Window类型
             self._app = app_or_driver._app
             if self._app:
                 self._driver = app_or_driver._app.get_driver(self.Process)
             else:
                 self._driver = app_or_driver._driver
             self._device = app_or_driver.device
 
         else:
             # AndroidDriver类型，一般用于调试
             self._driver = app_or_driver
-        
+
         if not isinstance(self._driver, AndroidDriver):
-            raise RuntimeError('参数类型错误：%s' % self._driver.__class__)
+            raise RuntimeError("参数类型错误：%s" % self._driver.__class__)
         self._wait_activity = wait_activity
         if wait_activity:
-            self._wait_timeout = kwds.get('wait_timeout')
-            self._wait_interval = kwds.get('wait_interval')
-        self._lazy_obj = LazyInit(self, '_lazy_obj', self._init_window)
+            self._wait_timeout = kwds.get("wait_timeout")
+            self._wait_interval = kwds.get("wait_interval")
+        self._lazy_obj = LazyInit(self, "_lazy_obj", self._init_window)
 
     def _init_window(self):
-        '''延迟初始化时执行
-        '''
+        """延迟初始化时执行
+        """
         self._lazy_obj = self  # 避免多次调用初始化函数
         if self._wait_activity == True:
             wait_timeout = self._wait_timeout
-            if not wait_timeout: wait_timeout = 12
+            if not wait_timeout:
+                wait_timeout = 12
             wait_interval = self._wait_interval
-            if not wait_interval: wait_interval = 0.5
+            if not wait_interval:
+                wait_interval = 0.5
             self.wait_for_exist(wait_timeout, wait_interval)
         self.post_init()
         return self
-    
+
     def post_init(self):
-        '''窗口类自定义的初始化逻辑
-        '''
+        """窗口类自定义的初始化逻辑
+        """
         pass
-    
+
     @property
     def Controls(self):
-        '''返回控件集合。使用如foo.Controls['最小化按钮']的形式获取控件
-        '''
+        """返回控件集合。使用如foo.Controls['最小化按钮']的形式获取控件
+        """
         return self
-    
+
     def hasControlKey(self, control_key):
-        '''是否包含控件control_key
+        """是否包含控件control_key
         
         :rtype: boolean
-        '''
-        return (control_key in self._locators)
-    
+        """
+        return control_key in self._locators
+
     @property
     def device(self):
         return self._device
 
     def __findctrl_recur(self, ctrlkey):
         if not (ctrlkey in self._locators.keys()):
             raise NameError("%s没有名为'%s'的子控件！" % (type(self), ctrlkey))
         params = self._locators[ctrlkey].copy()
-        ctrltype = params['type']
-        del params['type']
+        ctrltype = params["type"]
+        del params["type"]
         for key in params:
             value = params[key]
-            if isinstance(value, six.string_types) and value.startswith('@'):
+            if isinstance(value, six.string_types) and value.startswith("@"):
                 params[key] = self[value[1:]]  # 使用缓存
         if issubclass(ctrltype, View):
             return ctrltype(**params)
         else:
-            root = params.pop('root', None)
-            if root == None: root = self
-            params.pop('driver', None)  # delete unexpected param
-            params.pop('activity', None)
+            root = params.pop("root", None)
+            if root == None:
+                root = self
+            params.pop("driver", None)  # delete unexpected param
+            params.pop("activity", None)
             return ctrltype(root, ctrlkey, **params)
-            
+
     @lazy_init
     def __getitem__(self, index):
-        '''获取index指定控件
+        """获取index指定控件
         
         :type index: string
         :param index: 控件索引，如'查找按钮'  
-        '''
+        """
         if not (index in self._locators.keys()):
             raise NameError("%s没有名为'%s'的子控件！" % (type(self), index))
-        if not '_instance' in self._locators[index]:
+        if not "_instance" in self._locators[index]:
             instance = self.__findctrl_recur(index)
-            self._locators[index]['_instance'] = instance
-        return self._locators[index]['_instance']
-    
-    @Deprecated('update_locator')
+            self._locators[index]["_instance"] = instance
+        return self._locators[index]["_instance"]
+
+    @Deprecated("update_locator")
     def updateLocator(self, locators):
         self.update_locator(locators)
-    
+
     def update_locator(self, locators):
-        '''更新控件定义
-        '''
+        """更新控件定义
+        """
         for key in locators.keys():
-            locators[key]['driver'] = self._driver  # 保存driver实例
-            locators[key]['activity'] = self.__class__.Activity
+            locators[key]["driver"] = self._driver  # 保存driver实例
+            if "activity" not in locators[key]:
+                locators[key]["activity"] = self.__class__.Activity
         self._locators.update(locators)
-        
+
     def wait_for_exist(self, timeout=10, interval=0.5):
-        '''等待窗口出现
-        '''
+        """等待窗口出现
+        """
         import re
+
         time0 = time.time()
-        current_activity = ''
-        if self.Activity == '': return True
+        current_activity = ""
+        if self.Activity == "":
+            return True
         pattern = re.compile(self.Activity)
         while time.time() - time0 < timeout:
             current_activity = self.device.current_activity
             if current_activity == self.Activity:
                 return True
             if current_activity and pattern.match(current_activity):
                 return True
             time.sleep(interval)
-        raise ControlNotFoundError('窗口：%s 未找到，当前窗口为：%s' % (self.__class__.Activity, current_activity))
-    
+        raise ControlNotFoundError(
+            "窗口：%s 未找到，当前窗口为：%s" % (self.__class__.Activity, general_encode(current_activity))
+        )
+
     @property
     @lazy_init
     def rect(self):
-        '''窗口区域
-        '''
+        """窗口区域
+        """
         root = self._driver.get_control(self.Activity, None, [])
         if root == 0:
-            raise RuntimeError('查找根节点失败')
+            raise RuntimeError("查找根节点失败")
         rect = self._driver.get_control_rect(root)
-        return rect['Left'], rect['Top'], rect['Width'], rect['Height']
+        return rect["Left"], rect["Top"], rect["Width"], rect["Height"]
 
     @lazy_init
     def close(self):
-        '''关闭窗口
-        '''
-        if self.Activity == '':
-            self._driver.send_key('{BACK}')
+        """关闭窗口
+        """
+        if self.Activity == "":
+            self._driver.send_key("{BACK}")
         else:
             if not self._driver.close_activity(self.Activity):
-                self._driver.send_key('{BACK}')
+                self._driver.send_key("{BACK}")
 
         timeout = 3
         time0 = time.time()
         while time.time() - time0 < timeout:
-            if self.device.current_activity != self.Activity: return
+            if self.device.current_activity != self.Activity:
+                return
             time.sleep(0.5)
-    
+
     def get_metis_view(self):
-        '''返回MetisView
-        '''
+        """返回MetisView
+        """
         from qt4a.mtcontrols import MetisView
+
         return MetisView(self)
-    
+
+
 class Gravity(object):
-    '''用于控制控件靠左、居中等位置的属性
-    '''
+    """用于控制控件靠左、居中等位置的属性
+    """
+
     NO_GRAVITY = 0x0000
     AXIS_SPECIFIED = 0x0001
     AXIS_PULL_BEFORE = 0x0002
     AXIS_PULL_AFTER = 0x0004
     AXIS_CLIP = 0x0008
     AXIS_X_SHIFT = 0
     AXIS_Y_SHIFT = 4
@@ -222,16 +239,20 @@
     CENTER_HORIZONTAL = AXIS_SPECIFIED << AXIS_X_SHIFT
     FILL_HORIZONTAL = LEFT | RIGHT
     CENTER = CENTER_VERTICAL | CENTER_HORIZONTAL
     FILL = FILL_VERTICAL | FILL_HORIZONTAL
     CLIP_VERTICAL = AXIS_CLIP << AXIS_Y_SHIFT
     CLIP_HORIZONTAL = AXIS_CLIP << AXIS_X_SHIFT
     RELATIVE_LAYOUT_DIRECTION = 0x00800000
-    HORIZONTAL_GRAVITY_MASK = (AXIS_SPECIFIED | AXIS_PULL_BEFORE | AXIS_PULL_AFTER) << AXIS_X_SHIFT
-    VERTICAL_GRAVITY_MASK = (AXIS_SPECIFIED | AXIS_PULL_BEFORE | AXIS_PULL_AFTER) << AXIS_Y_SHIFT
+    HORIZONTAL_GRAVITY_MASK = (
+        AXIS_SPECIFIED | AXIS_PULL_BEFORE | AXIS_PULL_AFTER
+    ) << AXIS_X_SHIFT
+    VERTICAL_GRAVITY_MASK = (
+        AXIS_SPECIFIED | AXIS_PULL_BEFORE | AXIS_PULL_AFTER
+    ) << AXIS_Y_SHIFT
     DISPLAY_CLIP_VERTICAL = 0x10000000
     DISPLAY_CLIP_HORIZONTAL = 0x01000000
     START = RELATIVE_LAYOUT_DIRECTION | LEFT
     END = RELATIVE_LAYOUT_DIRECTION | RIGHT
     RELATIVE_HORIZONTAL_GRAVITY_MASK = START | END
 
     def __init__(self, grav):
@@ -247,225 +268,260 @@
 
     @property
     def center(self):
         raise NotImplementedError()
 
 
 def func_wrap(func):
-    '''用于方法包装，主要作用是发现控件失效时能够更新控件
-    '''
+    """用于方法包装，主要作用是发现控件失效时能够更新控件
+    """
+
     def _func(*args, **kwargs):
         from qt4a.androiddriver.util import logger, ControlExpiredError
+
         try:
             return func(*args, **kwargs)
         except ControlExpiredError as e:
             view = args[0]
             try:
                 view._update()
             except RuntimeError:
-                logger.exception('update control failed')
+                logger.exception("update control failed")
                 raise e  # 更新失败时直接抛出控件失效异常
             return func(*args, **kwargs)
+
     return _func
 
+
 class VerticalSwipe(object):
-    '''纵向滑动包装类
-    '''
+    """纵向滑动包装类
+    """
+
     def __init__(self, view):
         self._view = view
         self._is_class = isinstance(view, type)
-        
+
     def __call__(self, *args, **kwds):
         if not self._is_class:
-            raise RuntimeError('对象不支持__call__')
+            raise RuntimeError("对象不支持__call__")
         view = self._view(*args, **kwds)
         return VerticalSwipe(view)
-    
+
     def __str__(self):
         if not self._is_class:
-            return '<VerticalSwipe_%s object at 0x%.8X>' % (self._view.__class__.__name__, id(self))
+            return "<VerticalSwipe_%s object at 0x%.8X>" % (
+                self._view.__class__.__name__,
+                id(self),
+            )
         else:
-            return '<class \'VerticalSwipe_%s\'>' % self._view.__name__
-        
+            return "<class 'VerticalSwipe_%s'>" % self._view.__name__
+
     @property
     def rect(self):
-        '''left, top, width, height
-        '''
+        """left, top, width, height
+        """
         self_rect = self._view.rect
         root = self._view._root
 
         root_list = []
         while not isinstance(root, Window):
             if isinstance(root, ScrollView):
                 root_list.append(root)
             root = root._root
-            
-        if len(root_list) == 0: return self_rect
+
+        if len(root_list) == 0:
+            return self_rect
         root_rect = root_list[-1].rect  # 获取可滚动的最顶层根
         left = self_rect[0] if self_rect[0] > root_rect[0] else root_rect[0]
         top = self_rect[1] if self_rect[1] > root_rect[1] else root_rect[1]
-        width = self_rect[0] + self_rect[2] - left if self_rect[0] + self_rect[2] < root_rect[0] + root_rect[2] else root_rect[0] + root_rect[2] - left
-        height = self_rect[1] + self_rect[3] - top if self_rect[1] + self_rect[3] < root_rect[1] + root_rect[3] else root_rect[1] + root_rect[3] - top
+        width = (
+            self_rect[0] + self_rect[2] - left
+            if self_rect[0] + self_rect[2] < root_rect[0] + root_rect[2]
+            else root_rect[0] + root_rect[2] - left
+        )
+        height = (
+            self_rect[1] + self_rect[3] - top
+            if self_rect[1] + self_rect[3] < root_rect[1] + root_rect[3]
+            else root_rect[1] + root_rect[3] - top
+        )
         return left, top, width, height  # 取交集
-        
+
     def swipe_up(self):
-        '''向上滑动
-        '''
+        """向上滑动
+        """
         rect = self.rect
         x1 = x2 = rect[0] + rect[2] // 2
         y1 = rect[1] + rect[3] * 3 // 4
         y2 = rect[1] + rect[3] // 4
         self._view._driver.drag(x1, y1, x2, y2)
-    
+
     def swipe_down(self):
-        '''向下滑动
-        '''
+        """向下滑动
+        """
         rect = self.rect
         x1 = x2 = rect[0] + rect[2] // 2
         y1 = rect[1] + rect[3] // 4
         y2 = rect[1] + rect[3] * 3 // 4
         self._view._driver.drag(x1, y1, x2, y2)
-    
+
     def __getattr__(self, attr):
         return getattr(self._view, attr)
-    
+
+
 class View(object):
-    '''控件基类
-    '''
+    """控件基类
+    """
+
     def __init__(self, activity, root, driver, locator=None, hashcode=0):
         self._root = root
         if locator != None:
             self._qpath = locator
             self._locator = locator._parsed_qpath  # 解析后的list
         else:
             if hashcode == 0:
-                raise RuntimeError('参数错误')
+                raise RuntimeError("参数错误")
             self._locator = []
         self._driver = driver
         self._activity = activity
         self._hashcode = 0  # 每个Java对象实例的hashcode（根据内存地址计算出来）
         if hashcode != 0:
             self._hashcode = hashcode
         self._need_convert_qpath = True  # 是否需要转换QPath的ID为整型ID
-        
+
     def __eq__(self, other):
-        '''根据hashcode判断两个控件是否相同
-        '''
-        if other == None: return False
+        """根据hashcode判断两个控件是否相同
+        """
+        if other == None:
+            return False
         if self.hashcode == 0 or other.hashcode == 0:
-            raise RuntimeError('hashcode错误')
+            raise RuntimeError("hashcode错误")
         return self.hashcode == other.hashcode
 
     def __str__(self):
-        return '<%s(id=0x%X) at 0x%X>' % (self.__class__.__name__, self.hashcode & 0xFFFFFFFF, id(self))
-    
+        return "<%s(id=0x%X) at 0x%X>" % (
+            self.__class__.__name__,
+            self.hashcode & 0xFFFFFFFF,
+            id(self),
+        )
+
     def _handle_qpath(self, qpath):
-        '''对qpath进行处理，返回处理过的QPath列表
-        '''
+        """对qpath进行处理，返回处理过的QPath列表
+        """
         # 将字符串ID改为整型ID
         import copy, itertools
+
         qpath = copy.deepcopy(qpath)  # 防止qpath被修改
-        
+
         result = []  # 返回的是可能的qpath的列表
         for item in qpath:
             item_list = []
-            if 'Id' in item:
+            if "Id" in item:
                 # TODO: 如果有两级ID，其中一级是数字形式的
-                id_list = self.container._app._get_view_id(item['Id'][1])  # 可能会有多个整型ID
-                if id_list == None: 
+                id_list = self.container._app._get_view_id(item["Id"][1])  # 可能会有多个整型ID
+                if id_list == None:
                     item_list.append(item)
                     result.append(item_list)
                     continue
                 if len(id_list) == 1:
-                    item['Id'][1] = str(id_list[0])
+                    item["Id"][1] = str(id_list[0])
                     item_list.append(item)
                 else:
                     # 存在多个id
                     for _id in id_list:
-                        item['Id'][1] = str(_id)
+                        item["Id"][1] = str(_id)
                         item_list.append(copy.deepcopy(item))
             else:
                 item_list.append(item)
             result.append(item_list)
-            
+
         qpath_list = []
         for qpath in itertools.product(*result):
             qpath_list.append(qpath)
         return qpath_list
-    
+
     @property
     def container(self):
-        '''获取所在容器类
-        '''
+        """获取所在容器类
+        """
         root = self._root
         if isinstance(root, Window):
             return root
         else:
             return root.container
 
     def _get_hashcode(self, parent=0, locator=None):
-        '''找到控件的hashcode值
-        '''
-        if locator: self._locator = locator
-        if not self._locator: raise RuntimeError('控件定位信息缺失')
+        """找到控件的hashcode值
+        """
+        if locator:
+            self._locator = locator
+        if not self._locator:
+            raise RuntimeError("控件定位信息缺失")
         if parent == 0 and isinstance(self._root, View):
             # 存在父节点
             if self._root._hashcode != 0:
                 parent = self._root._hashcode
             else:
                 parent = self._root._get_hashcode()
-                if parent == 0: return 0  # 父节点不存在
+                if parent == 0:
+                    return 0  # 父节点不存在
                 self._root._hashcode = parent
-        
+
         idx = 0
         if isinstance(self._locator, list):
             # 先使用原始QPath查询一次
             result = self._driver.get_control(self._activity, parent, self._locator)
-            if result != 0: 
-                if self._need_convert_qpath: self._need_convert_qpath = False  # 不再需要转换QPath
+            if result != 0:
+                if self._need_convert_qpath:
+                    self._need_convert_qpath = False  # 不再需要转换QPath
                 return result  # TODO: 处理"控件索引超出范围"情况
-            if not self._need_convert_qpath: return 0  # 避免控件消失后还要再去获取整型ID
-            if not self.container._app._is_use_int_view_id(): return 0  # 不使用整型ID
-            
+            if not self._need_convert_qpath:
+                return 0  # 避免控件消失后还要再去获取整型ID
+            if not self.container._app._is_use_int_view_id():
+                return 0  # 不使用整型ID
+
             import re
-            pattern = re.compile('^0x[0-9a-fA-F]+$')
-            
+
+            pattern = re.compile("^0x[0-9a-fA-F]+$")
+
             need_convert = False
             for item in self._locator:
-                if 'Id' in item:
-                    if item['Id'][1].isdigit(): continue
-                    if pattern.match(item['Id'][1]): continue  # 16进制的
+                if "Id" in item:
+                    if item["Id"][1].isdigit():
+                        continue
+                    if pattern.match(item["Id"][1]):
+                        continue  # 16进制的
                     need_convert = True
                     break
-            if not need_convert: return 0  # 已经是数字类型的ID了
-            
+            if not need_convert:
+                return 0  # 已经是数字类型的ID了
+
             # 生成整型ID的QPath
-            qpath_list = self._handle_qpath(self._locator)  
+            qpath_list = self._handle_qpath(self._locator)
             if len(qpath_list) == 1:
                 self._locator = (self._locator, qpath_list[0])
             elif len(qpath_list) > 1:
                 # 有多个QPath
                 qpath_list.insert(0, self._locator)
                 self._locator = tuple(qpath_list)  # tuple类型
             else:
-                raise RuntimeError('QPath解析错误：%s' % self._locator)
+                raise RuntimeError("QPath解析错误：%s" % self._locator)
             idx = 1  # 第一个不需要检查了
-            
+
         for loc in self._locator[idx:]:
             result = self._driver.get_control(self._activity, parent, loc)
-            if result != 0: 
+            if result != 0:
                 self._locator = list(loc)  # 如果找到,认为这是正确的QPath,以后只使用该QPath进行查找
                 self._need_convert_qpath = False
                 return result  # 找到即返回
         return 0
-            
+
     @property
     def hashcode(self):
-        '''控件唯一标识，只有真正访问控件信息时才会去获取该标识
-        '''
+        """控件唯一标识，只有真正访问控件信息时才会去获取该标识
+        """
         if self._hashcode == 0:
             # 尚未获取控件的hashcode
             timeout = 10  # 查找控件的超时时间
             interval = 0.1
             time0 = time.time()
             while time.time() - time0 < timeout:
                 self._hashcode = self._get_hashcode()
@@ -492,218 +548,266 @@
                             break
                 parent = parent._hashcode if isinstance(parent, View) else 0
                 pos = self._driver.get_control(self._activity, parent, locator, True)
                 qpath = str(qpath)
                 split_char = qpath[0]
                 qpath_list = qpath[1:].split(split_char)
                 err_qpath = split_char.join(qpath_list[pos:])
-                if err_qpath: err_qpath = split_char + err_qpath  # 补上前面的分隔符
-                err_msg = '进程【%s】中未找到控件：%s \n未找到部分路径为：【%s】' % (self._driver._process_name, qpath, err_qpath)
+                if err_qpath:
+                    err_qpath = split_char + err_qpath  # 补上前面的分隔符
+                err_msg = "进程【%s】中未找到控件：%s \n未找到部分路径为：【%s】" % (
+                    self._driver._process_name,
+                    qpath,
+                    err_qpath,
+                )
                 current_activity = self.container.device.get_current_activity()
                 view_tree = self._driver.get_control_tree(current_activity)
-                logger.info('Current acvitiy %s control tree：\n%s' % (current_activity.encode('utf8'), view_tree.encode('utf8')))
+                logger.info(
+                    "Current acvitiy %s control tree：\n%s"
+                    % (current_activity.encode("utf8"), view_tree.encode("utf8"))
+                )
                 raise ControlNotFoundError(err_msg)
         return self._hashcode
 
     def _update(self):
-        '''更新hashcode
-        '''
+        """更新hashcode
+        """
         if isinstance(self._root, View):
             self._root._update()
         self._hashcode = 0
         return self.hashcode
 
     @property
     @func_wrap
     def parent(self):
-        '''获取父控件
-        '''
-        if not hasattr(self, '_parent'):
+        """获取父控件
+        """
+        if not hasattr(self, "_parent"):
             self._parent = self._driver.get_parent(self.hashcode)
-        return View(hashcode=self._parent, activity=self._activity, root=self.container, driver=self._driver)
+        return View(
+            hashcode=self._parent,
+            activity=self._activity,
+            root=self.container,
+            driver=self._driver,
+        )
 
     @property
     @func_wrap
     def children(self):
-        '''获取子节点列表
-        '''
+        """获取子节点列表
+        """
         children = self._driver.get_children(self.hashcode)
-        return [View(hashcode=child, root=self, activity=self._activity, driver=self._driver) for child in children]
+        return [
+            View(
+                hashcode=child, root=self, activity=self._activity, driver=self._driver
+            )
+            for child in children
+        ]
 
     @property
     @func_wrap
     def rect(self):
-        '''left, top, width, height
-        '''
+        """left, top, width, height
+        """
         get_rect_interval = 0.1  # 防止频繁获取控件坐标信息
-        if not hasattr(self, '_last_get_rect_time') or (time.time() - self._last_get_rect_time) > get_rect_interval:
+        if (
+            not hasattr(self, "_last_get_rect_time")
+            or (time.time() - self._last_get_rect_time) > get_rect_interval
+        ):
             rect = self._driver.get_control_rect(self.hashcode)
-            result = rect['Left'], rect['Top'], rect['Width'], rect['Height']
+            result = rect["Left"], rect["Top"], rect["Width"], rect["Height"]
             self._last_get_rect_time = time.time()
             self._last_rect = result
         return self._last_rect
 
     @property
     @func_wrap
     def visible(self):
-        '''是否可见
-        '''
+        """是否可见
+        """
         return self._driver.get_control_visibility(self.hashcode)
 
     @property
     @func_wrap
     def _clickable(self):
-        '''是否可点击
-        '''
+        """是否可点击
+        """
         CLICKABLE = 0x00004000
-        flags = self._driver.get_object_field_value(self.hashcode, 'mViewFlags')
+        flags = self._driver.get_object_field_value(self.hashcode, "mViewFlags")
         return int(flags) & CLICKABLE == CLICKABLE
 
     @property
     def clickable(self):
-        '''是否可点击
+        """是否可点击
         to be deleted
-        '''
+        """
         return self._clickable
 
     @property
     @func_wrap
     def enabled(self):
-        '''是否可用
-        '''
+        """是否可用
+        """
         ENABLE = 0x00000000
         ENABLED_MASK = 0x00000020
-        flags = int(self._driver.get_object_field_value(self.hashcode, 'mViewFlags'))
+        flags = int(self._driver.get_object_field_value(self.hashcode, "mViewFlags"))
         return flags & ENABLED_MASK == ENABLE
 
     @property
     @func_wrap
     def background_color(self):
-        '''背景色
-        '''
-        result = self._driver.get_object_field_value(self.hashcode, 'mBackground.mColorState.mUseColor')
-        if result == 'null':
+        """背景色
+        """
+        result = self._driver.get_object_field_value(
+            self.hashcode, "mBackground.mColorState.mUseColor"
+        )
+        if result == "null":
             return None
         return int(result)
 
     @property
     def content_desc(self):
-        '''控件描述
-        '''
-        return self._driver.get_object_field_value(self.hashcode, 'mContentDescription')
-    
+        """控件描述
+        """
+        return self._driver.get_object_field_value(self.hashcode, "mContentDescription")
+
     def exist(self):
-        '''判断控件是否存在
-        '''
+        """判断控件是否存在
+        """
         from qt4a.androiddriver.util import ControlExpiredError, logger
+
         try:
             self._hashcode = self._get_hashcode()
             return self._hashcode != 0  # 由于Java端使用int型存储，因此可能为负数
         except ControlExpiredError:
             return False
         except RuntimeError:
-            logger.exception('获取控件失败')  # 如果没有获取到控件ID对应的整型ID，认为控件不存在
+            logger.exception("获取控件失败")  # 如果没有获取到控件ID对应的整型ID，认为控件不存在
             return False
-        
+
     def wait_for_exist(self, timeout=10, interval=0.1):
-        '''等待控件出现
-        '''
+        """等待控件出现
+        """
         time0 = time.time()
         while time.time() - time0 < timeout:
-            if self.exist(): return True
+            if self.exist():
+                return True
             time.sleep(interval)
-        raise ControlNotFoundError('控件：%s 未找到' % self._qpath)
+        raise ControlNotFoundError("控件：%s 未找到" % self._qpath)
 
     def wait_for_visible(self, timeout=10, interval=0.2):
-        '''等待控件可见
+        """等待控件可见
         
         :param timeout:  超时时间，单位：秒
         :type  timeout:  int/float
         :param interval: 重试间隔时间，单位：秒
         :type  interval: int/float
-        '''
+        """
         time0 = time.time()
         while time.time() - time0 < timeout:
-            if self.visible: return
+            if self.visible:
+                return
             time.sleep(interval)
-        raise RuntimeError('Control is not visible in %s seconds' % timeout)
-    
+        raise RuntimeError("Control is not visible in %s seconds" % timeout)
+
     def wait_for_invisible(self, timeout=10, interval=0.2):
-        '''等待控件不可见
+        """等待控件不可见
         
         :param timeout:  超时时间，单位：秒
         :type  timeout:  int/float
         :param interval: 重试间隔时间，单位：秒
         :type  interval: int/float
-        '''
+        """
         time0 = time.time()
         while time.time() - time0 < timeout:
-            if not self.visible: return
+            if not self.visible:
+                return
             time.sleep(interval)
-        raise RuntimeError('Control is not invisible in %s seconds' % timeout)
-    
+        raise RuntimeError("Control is not invisible in %s seconds" % timeout)
+
     def _point_in_view(self, x, y):
-        '''判断点(x, y)是否在当前View可视范围内
-        '''
+        """判断点(x, y)是否在当前View可视范围内
+        """
         view_rect = self.rect
-        if x < view_rect[0] or x >= view_rect[0] + view_rect[2]: return False
-        if y < view_rect[1] or y >= view_rect[1] + view_rect[3]: return False
+        if x < view_rect[0] or x >= view_rect[0] + view_rect[2]:
+            return False
+        if y < view_rect[1] or y >= view_rect[1] + view_rect[3]:
+            return False
         return True
-    
+
     def _get_scroll_root(self):
-        '''获取当前控件可滚动区域的根控件
-        '''
+        """获取当前控件可滚动区域的根控件
+        """
         root = self._root
         if isinstance(root, ListItem):
             root = root._root  # 获取ListView视图
 
         root_list = []
         while not isinstance(root, Window):
             if isinstance(root, (ScrollView, ViewPager)):
                 root_list.append(root)
             root = root._root
-        if root_list == []: return None
+        if root_list == []:
+            return None
         return root_list[-1]  # 获取可滚动的最顶层根
-        
+
     def scroll_to_visible(self, root_rect=None, self_rect=None):
-        '''滚动到可视区域
-        '''
+        """滚动到可视区域
+        """
         root = self._get_scroll_root()
-        if root == None: return 0, 0  # 不需要滚动
-        
-        if not self_rect: self_rect = self.rect
-        if not root_rect: root_rect = root.rect
+        if root == None:
+            return 0, 0  # 不需要滚动
+
+        if not self_rect:
+            self_rect = self.rect
+        if not root_rect:
+            root_rect = root.rect
         visible_rect = get_intersection(self_rect, root_rect)
         min_clickable_area = (20, 10)  # 最小可点击区域的大小
         _, screen_height = self.container.device.screen_size
-        if visible_rect[0] >= 0 and visible_rect[1] >= 0 and visible_rect[2] >= min_clickable_area[0] and visible_rect[3] >= min_clickable_area[1] and screen_height - (visible_rect[1] + visible_rect[3]) >= 50: 
-            logger.info('intersect area is %s' % (visible_rect,))
+        if (
+            visible_rect[0] >= 0
+            and visible_rect[1] >= 0
+            and visible_rect[2] >= min_clickable_area[0]
+            and visible_rect[3] >= min_clickable_area[1]
+            and screen_height - (visible_rect[1] + visible_rect[3]) >= 50
+        ):
+            logger.info("intersect area is %s" % (visible_rect,))
             return 0, 0
-        
+
         if self_rect[2] > root_rect[2] or self_rect[3] > root_rect[3]:
             x_visible = True
             y_visible = True
             if self_rect[2] >= root_rect[2]:
                 # 控件宽度大于容器宽度
                 max_left = self_rect[0] if self_rect[0] > root_rect[0] else root_rect[0]
-                min_right = self_rect[0] + self_rect[2] if self_rect[0] + self_rect[2] < root_rect[0] + root_rect[2] else root_rect[0] + root_rect[2]
+                min_right = (
+                    self_rect[0] + self_rect[2]
+                    if self_rect[0] + self_rect[2] < root_rect[0] + root_rect[2]
+                    else root_rect[0] + root_rect[2]
+                )
                 visible_width = min_right - max_left
                 if visible_width < root_rect[2] // 2:
                     # 由于此时控件不可能完全可见，因此认为一半可见即为可见
                     x_visible = False
             if self_rect[3] >= root_rect[3]:
                 # 控件高度大于容器高度
                 max_top = self_rect[1] if self_rect[1] > root_rect[1] else root_rect[1]
-                min_bottom = self_rect[1] + self_rect[3] if self_rect[1] + self_rect[3] < root_rect[1] + root_rect[3] else root_rect[1] + root_rect[3]
+                min_bottom = (
+                    self_rect[1] + self_rect[3]
+                    if self_rect[1] + self_rect[3] < root_rect[1] + root_rect[3]
+                    else root_rect[1] + root_rect[3]
+                )
                 visible_height = min_bottom - max_top
                 if visible_height < root_rect[3] // 2:
                     y_visible = False
 
-            if x_visible and y_visible: return 0, 0
-            
+            if x_visible and y_visible:
+                return 0, 0
+
         # print (self_rect, root_rect)
 
         if isinstance(root, ViewPager):
             offset = self_rect[0] - root_rect[0]
             count = offset // root_rect[2]
             root.scroll(count, root_rect)
             return root_rect[2] * count, 0
@@ -726,46 +830,52 @@
             # 低于5个像素不滚动
             # print (x_offset, y_offset)
             root.scroll(x_offset, y_offset)
             time.sleep(0.5)  # 测试发现，滑动后等待时间过短就点击会无效
         return x_offset, y_offset
 
     def _pre_click(self, x_offset=None, y_offset=None):
-        '''点击前的处理
+        """点击前的处理
         
         :param x_offset: 距离控件区域左上角的横向偏移。
         :type x_offset:  int或float
         :param y_offset: 距离控件区域左上角的纵向偏移。
         :type y_offset:  int或float
         
         :return 要点击的坐标
-        '''
+        """
 
         visible = False
         rect_valid = False
         old_rect = None
         enable = False
-        
+
         screen_width, screen_height = self.container.device.screen_size
         self.hashcode  # 确保控件存在
         root = self._get_scroll_root()
         root_rect = root.rect if root != None else [0, 0, screen_width, screen_height]
         if root != None:
             timeout = 2
             time0 = time.time()
             while time.time() - time0 < timeout:
-                if root_rect[2] == 0 or root_rect[3] == 0 or root_rect[0] < 0 or root_rect[1] < 0 or \
-                root_rect[0] + root_rect[2] > screen_width or root_rect[1] + root_rect[3] > screen_height:
+                if (
+                    root_rect[2] == 0
+                    or root_rect[3] == 0
+                    or root_rect[0] < 0
+                    or root_rect[1] < 0
+                    or root_rect[0] + root_rect[2] > screen_width
+                    or root_rect[1] + root_rect[3] > screen_height
+                ):
                     time.sleep(0.1)
                     root_rect = root.rect
                 else:
                     break
             else:
-                logger.warn('invalid root rect: %s' % (root_rect,))
-                
+                logger.warn("invalid root rect: %s" % (root_rect,))
+
         timeout = 10
         time0 = time.time()
         while time.time() - time0 < timeout:
             # 尝试操作，会出现由于控件尚未初始化完成导致获取的rect不正确的情况
             if not visible:
                 if not self.visible:
                     time.sleep(0.1)
@@ -775,691 +885,770 @@
 
             if not enable:
                 # 检查是否可用
                 enable = self.enabled
                 if not enable:
                     time.sleep(0.1)
                     continue
-            
+
             if not rect_valid:
                 rect = self.rect
                 if rect[2] == 0 or rect[3] == 0:  # 进行点击操作的控件长宽不可能为0
-                    logger.debug('control %s width or height is 0 [%s]' % (self._hashcode, rect))
+                    logger.debug(
+                        "control %s width or height is 0 [%s]" % (self._hashcode, rect)
+                    )
                     time.sleep(0.2)  # 间隔时间延长为0.2S
                     continue
-                
+
                 if not old_rect or rect != old_rect:
                     # 等待控件坐标稳定
                     old_rect = rect
-                    logger.debug('wait for control %s stable' % self._hashcode)
+                    logger.debug("wait for control %s stable" % self._hashcode)
                     time.sleep(0.2)
                     continue
-                
+
                 is_scroll = False  # 控件是否滚动
                 if root != None:
                     for _ in range(5):
-                        x_offset1, y_offset1 = self.scroll_to_visible(root_rect, rect)  # 自动滚动到可视区域
+                        x_offset1, y_offset1 = self.scroll_to_visible(
+                            root_rect, rect
+                        )  # 自动滚动到可视区域
                         if abs(x_offset1) <= 5 and abs(y_offset1) <= 5:
                             break
                         else:
                             is_scroll = True
                             rect = self.rect  # 重新获取滚动后的坐标
-                
+
                 visible_rect = get_intersection(rect, root_rect)
                 if is_scroll:
                     old_rect = visible_rect
                     time.sleep(0.2)
                 else:
                     # 不需要再判断控件是否稳定
                     old_rect = None
                     rect = visible_rect
                 rect_valid = True
-            
+
             if old_rect != None:
                 rect = get_intersection(self.rect, root_rect)
                 if old_rect != rect:
                     # 防止有些控件加载后出现位移
                     old_rect = rect
                     time.sleep(0.2)
                     continue
-            
-            x = (rect[0] + rect[2] // 2)
-            y = (rect[1] + rect[3] // 2)
-            if x_offset: x = rect[0] + x_offset
-            if y_offset: y = rect[1] + y_offset
+
+            x = rect[0] + rect[2] // 2
+            y = rect[1] + rect[3] // 2
+            if x_offset:
+                x = rect[0] + x_offset
+            if y_offset:
+                y = rect[1] + y_offset
             return x, y
         else:
             current_activity = self.container.device.get_current_activity()
             if current_activity != self._activity:
                 import re
+
                 ret = re.compile(self._activity)
-                if not ret.match(current_activity): raise RuntimeError("当前Activity为%s，不是控件所属的Activity" % current_activity)
-            if not visible: raise RuntimeError('控件不可见')
-            if not enable: raise RuntimeError('控件不可用')
-            if not rect_valid: raise RuntimeError('控件区域错误')
-            raise RuntimeError('未知错误')
-    
+                if not ret.match(current_activity):
+                    raise RuntimeError(
+                        "当前Activity为%s，不是控件所属的Activity" % current_activity
+                    )
+            if not visible:
+                raise RuntimeError("控件不可见")
+            if not enable:
+                raise RuntimeError("控件不可用")
+            if not rect_valid:
+                raise RuntimeError("控件区域错误")
+            raise RuntimeError("未知错误")
+
     def _click(self, click_time, x=None, y=None, check_ret=True):
-        '''具有重试逻辑的点击
+        """具有重试逻辑的点击
         
         :param click_time: 按住的时长，单位为秒
         :type click_time:  int/float
         :param x: 点击的横坐标
         :type x:  int/float
         :param y: 点击的纵坐标
         :type y:  int/float
         :param check_ret: 是否检查点击成功
         :type check_ret:  bool
-        '''
+        """
         if not x or not y:
             rect = self.rect
-            if not x: x = rect[0] + rect[2] // 2
-            if not y: y = rect[1] + rect[3] // 2
+            if not x:
+                x = rect[0] + rect[2] // 2
+            if not y:
+                y = rect[1] + rect[3] // 2
         for _ in range(10):
             ret = self._driver.click(self.hashcode, x, y, click_time)
-            if not check_ret or ret: return True
+            if not check_ret or ret:
+                return True
             time.sleep(0.5)
-        raise RuntimeError('click (%d, %d) 失败' % (x, y))
-    
+        raise RuntimeError("click (%d, %d) 失败" % (x, y))
+
     @func_wrap
     def click(self, x_offset=0, y_offset=0):
-        '''单击
+        """单击
         
         :param x_offset: 距离控件区域左上角的横向偏移。
         :type x_offset:  int或float
         :param y_offset: 距离控件区域左上角的纵向偏移。
         :type y_offset:  int或float
-        '''
+        """
         x, y = self._pre_click(x_offset, y_offset)
         self._click(0, x, y)
-    
+
     def double_click(self, x_offset=0, y_offset=0):
-        '''双击
+        """双击
         
         :param x_offset: 距离控件区域左上角的横向偏移。
         :type x_offset:  int或float
         :param y_offset: 距离控件区域左上角的纵向偏移。
         :type y_offset:  int或float
-        '''
+        """
         x, y = self._pre_click(x_offset, y_offset)
         self._click(0, x, y)
         self._click(0, x, y)
-        
+
     def multiple_click(self, count=3, x_offset=0, y_offset=0):
-        '''多次点击
+        """多次点击
         
         :param count: 点击多少次
         :type count:  int
         :param x_offset: 距离控件区域左上角的横向偏移。
         :type x_offset:  int或float
         :param y_offset: 距离控件区域左上角的纵向偏移。
         :type y_offset:  int或float
-        '''
-        if count < 1: return
+        """
+        if count < 1:
+            return
         x, y = self._pre_click(x_offset, y_offset)
         for _ in range(count):
             self._click(0, x, y)
-    
+
     @func_wrap
     def long_click(self, duration=1, x_offset=0, y_offset=0, sync=True):
-        '''长按
+        """长按
         
         :param duration: 按住时长，单位为秒
         :type duration:  int/float
         :param x_offset: 距离控件区域左上角的横向偏移。
         :type x_offset:  int/float
         :param y_offset: 距离控件区域左上角的纵向偏移。
         :type y_offset:  int/float
         :param sync:     是否是同步调用，为True表示等到长按结束才返回，False表示立即返回
         :type sync:      bool
-        '''
+        """
         x, y = self._pre_click(x_offset, y_offset)
         if sync:
             self._click(duration, x, y, False)  # 长按不检查回调
         else:
             import threading
+
             # 按下后立即返回
             self._driver.drag(x, y, x, y, 0, 0, True, False)
+
             def _delay_func():
                 time.sleep(duration)
                 self._driver.drag(x, y, x, y, 0, 0, False, True)
+
             t = threading.Thread(target=_delay_func, args=())
             t.start()
-            
-    def wait_for_value(self, prop_name, prop_value, timeout=10, interval=0.5, regularMatch=False):
+
+    def wait_for_value(
+        self, prop_name, prop_value, timeout=10, interval=0.5, regularMatch=False
+    ):
         """等待控件属性值出现, 如果属性为字符串类型，则使用正则匹配
         
         :param prop_name: 属性名字
         :param prop_value: 等待出现的属性值
         :param timeout: 超时秒数, 默认为10
         :param interval: 等待间隔，默认为0.5
         :param regularMatch: 参数 property_name和waited_value是否采用正则表达式的比较。默认为不采用（False）正则，而是采用恒等比较。
         """
-        Timeout(timeout, interval).waitObjectProperty(self, prop_name, prop_value, regularMatch)
-    
+        Timeout(timeout, interval).waitObjectProperty(
+            self, prop_name, prop_value, regularMatch
+        )
+
     def swipe(self, direct):
-        '''滑动
+        """滑动
         
         :param direct: 方向
         :type direct:  string，只能是“up”、“down”、“left”、“right”中的一个值
-        '''
+        """
         rect = self.rect
-        if direct == 'up':
+        if direct == "up":
             x1 = x2 = rect[0] + rect[2] // 2
             y1 = rect[1] + rect[3] * 2 // 3
             y2 = rect[1] + rect[3] // 3
-        elif direct == 'down':
+        elif direct == "down":
             x1 = x2 = rect[0] + rect[2] // 2
             y1 = rect[1] + rect[3] // 3
             y2 = rect[1] + rect[3] * 2 // 3
-        elif direct == 'left':
+        elif direct == "left":
             y1 = y2 = rect[1] + rect[3] // 2
             x1 = rect[0] + rect[2] * 2 // 3
             x2 = rect[0] + rect[2] // 3
-        elif direct == 'right':
+        elif direct == "right":
             y1 = y2 = rect[1] + rect[3] // 2
             x1 = rect[0] + rect[2] // 3
             x2 = rect[0] + rect[2] * 2 // 3
         else:
-            raise RuntimeError('direct参数只能是：up、down、left、right中的一个')  
+            raise RuntimeError("direct参数只能是：up、down、left、right中的一个")
         self._driver.drag(x1, y1, x2, y2)
-    
+
     def get_metis_view(self):
-        '''返回MetisView
-        '''
+        """返回MetisView
+        """
         from qt4a.mtcontrols import MetisView
+
         return MetisView(self)
-    
+
+
 class TextView(View):
-    '''包含Text的View 
-    '''
+    """包含Text的View 
+    """
+
     @property
     @func_wrap
     def text(self):
-        '''获取文本
-        '''
+        """获取文本
+        """
         return self._driver.get_control_text(self.hashcode)
-    
+
     @property
     def html_style_text(self):
-        '''HTML格式文本
-        '''
+        """HTML格式文本
+        """
         return self._driver.get_control_text(self.hashcode, True)
-    
+
     @text.setter
     def text(self, value):
-        '''设置文本
-        '''
+        """设置文本
+        """
         if not isinstance(value, six.string_types):
             value = str(value)
         if six.PY2 and not isinstance(value, unicode):
             try:
-                value = value.decode('utf8')
+                value = value.decode("utf8")
             except UnicodeDecodeError:
-                raise RuntimeError('参数编码错误：%r' % value)
+                raise RuntimeError("参数编码错误：%r" % value)
         self.wait_for_visible()
         self.disable_soft_input()  # 赋值前关闭软键盘
         for _ in range(3):
-            if self._driver.set_control_text(self.hashcode, value): return
+            if self._driver.set_control_text(self.hashcode, value):
+                return
             self.click()
-        raise RuntimeError('设置控件文本失败')
-    
+        raise RuntimeError("设置控件文本失败")
+
     @property
     def text_size(self):
-        '''字体大小
-        '''
-        ret = self._driver.call_object_method(self.hashcode, 'mTextPaint', 'getTextSize')
+        """字体大小
+        """
+        ret = self._driver.call_object_method(
+            self.hashcode, "mTextPaint", "getTextSize"
+        )
         return int(ret)
-    
+
     @property
     def text_color(self):
-        '''字体颜色
-        '''
+        """字体颜色
+        """
         import json
-        ret = json.loads(self._driver.get_object_field_value(self.hashcode, 'mCurTextColor'))
+
+        ret = json.loads(
+            self._driver.get_object_field_value(self.hashcode, "mCurTextColor")
+        )
         ret = int(ret)
-        if ret < 0: ret += 0x100000000
+        if ret < 0:
+            ret += 0x100000000
         return ret
-    
+
     @func_wrap
     def disable_soft_input(self):
-        '''禁用软键盘
-        '''
+        """禁用软键盘
+        """
         self._driver.enable_soft_input(self.hashcode, False)
-    
+
     def _get_char_rect(self, start_offset, end_offset):
-        '''根据字符偏移量计算区域坐标
+        """根据字符偏移量计算区域坐标
         
         :param start_offset: 起始字符偏移
         :type start_offset:  int
         :param end_offset:   结束字符偏移
         :type end_offset:    int
-        '''
+        """
         rect = self._driver.get_text_rect(self.hashcode, start_offset, end_offset)
-        return rect['Left'], rect['Top'], rect['Width'], rect['Height']
-    
+        return rect["Left"], rect["Top"], rect["Width"], rect["Height"]
+
     @property
     def hint_text(self):
-        '''空白提示文本
-        '''
-        return self._driver.get_object_field_value(self.hashcode, 'mHint')
-    
+        """空白提示文本
+        """
+        return self._driver.get_object_field_value(self.hashcode, "mHint")
+
     @property
     def image_resource_name(self):
-        '''图像资源名称
-        '''
+        """图像资源名称
+        """
         result = self._driver.get_control_image_resource(self.hashcode)
         for key in result:
-            result[key] = self.container._app._get_drawable_resource_origin_name(result[key])
+            result[key] = self.container._app._get_drawable_resource_origin_name(
+                result[key]
+            )
         return result
-    
+
     def click_clickable_span(self):
-        '''点击TextView中的ClickableSpan区域
-        '''
+        """点击TextView中的ClickableSpan区域
+        """
         import re
-        pattern = re.compile(r'^<p.*>(.|\n)*<span onclick>(.+)</span>(.*)</p>\s*$')
+
+        pattern = re.compile(r"^<p.*>(.|\n)*<span onclick>(.+)</span>(.*)</p>\s*$")
         html = self.html_style_text
         ret = pattern.match(html)
-        if not ret: raise RuntimeError('HTML文本格式错误: %r' % html)
+        if not ret:
+            raise RuntimeError("HTML文本格式错误: %r" % html)
         text = self.text
         start_offset = text.find(ret.group(2))
         end_offset = start_offset + len(ret.group(2))
         rect = self._get_char_rect(start_offset + 1, end_offset)
 
         textview_rect = self.rect
         x1 = textview_rect[0]
         y1 = textview_rect[1]
         x2 = rect[0] + rect[2] // 2
         y2 = rect[1] + rect[3] // 2
         self.click(x2 - x1, y2 - y1)
-        
+
+
 class EditText(TextView):
-    '''输入文本框
-    '''
+    """输入文本框
+    """
+
+    def send_keys(self, text):
+        self.send_text(text)
+
     def send_text(self, text):
-        '''输入按键，此方法不能输入中文和大写字母
-        '''
+        """输入按键，此方法不能输入中文和大写字母
+        """
         self.click()  # 先获取焦点
         time.sleep(0.1)
         self._driver.send_keys(text)
 
     def click(self):
-        '''click后自动关闭输入法
-        '''
+        """click后自动关闭输入法
+        """
         super(TextView, self).click()
         self.disable_soft_input()
         time.sleep(1)
 
+
 class Button(TextView):
-    '''按钮类
-    '''
+    """按钮类
+    """
+
     pass
 
+
 class CompoundButton(Button):
-    '''可选按钮，一般用于实现Switch
-    '''
+    """可选按钮，一般用于实现Switch
+    """
+
     @property
     @func_wrap
     def checked(self):
-        '''是否已选
-        '''
+        """是否已选
+        """
         return self._driver.get_control_checked(self.hashcode)
 
     @checked.setter
     def checked(self, check=True):
-        '''设置是否选择
-        '''
-        if self.checked == check: return
+        """设置是否选择
+        """
+        if self.checked == check:
+            return
         self.click()
 
+
 class RadioButton(CompoundButton):
-    '''单选按钮
-    '''
+    """单选按钮
+    """
+
     pass
 
+
 class CheckBox(CompoundButton):
-    '''选择按钮
-    '''
+    """选择按钮
+    """
+
     pass
 
+
 class CheckedTextView(TextView):
-    '''可选文本框
-    '''
+    """可选文本框
+    """
+
     @property
     def checked(self):
-        '''是否已选
-        '''
-        return self._driver.get_object_field_value(self.hashcode, 'mChecked') == 'true'
+        """是否已选
+        """
+        return self._driver.get_object_field_value(self.hashcode, "mChecked") == "true"
+
 
 class ImageView(View):
-    '''显示图片控件
-    '''
+    """显示图片控件
+    """
+
     @property
     @func_wrap
     def resource_name(self):
-        '''当前使用的图片资源名称
-        '''
+        """当前使用的图片资源名称
+        """
         ret = self._driver.get_control_background(self.hashcode)
-        if ret: return self.container._app._get_drawable_resource_origin_name(ret)
+        if ret:
+            return self.container._app._get_drawable_resource_origin_name(ret)
         res_name = self._driver.get_control_image_resource(self.hashcode)
         return self.container._app._get_drawable_resource_origin_name(res_name)
-    
-    def capture(self, save_path=''):
-        '''保存图片到本地
-        '''
+
+    def capture(self, save_path=""):
+        """保存图片到本地
+        """
         if not save_path:
             import tempfile, os
+
             tmp_path = tempfile.mkdtemp()
-            save_path = os.path.join(tmp_path, 'tmp.png')
-        
+            save_path = os.path.join(tmp_path, "tmp.png")
+
         for _ in range(3):
             pic_data = self._driver.capture_control(self.hashcode)
-            if len(pic_data) == 0: 
+            if len(pic_data) == 0:
                 time.sleep(1)
                 continue
-            f = open(save_path, 'wb')
+            f = open(save_path, "wb")
             f.write(pic_data)
             f.close()
             return save_path
-        
-        raise RuntimeError('获取控件截图失败')
-    
-    def save(self, save_path=''):
-        '''保存图片到本地
+
+        raise RuntimeError("获取控件截图失败")
+
+    def save(self, save_path=""):
+        """保存图片到本地
         to de deleted
-        '''
+        """
         return self.capture(save_path)
-    
+
+
 class ImageButton(ImageView):
     pass
 
 
 class DropdownView(View):
     pass
 
 
 # 布局类
 class ViewGroup(View):
     pass
 
+
 class FrameLayout(ViewGroup):
     pass
 
+
 class LinearLayout(ViewGroup):
     pass
 
+
 class RelativeLayout(ViewGroup):
-    '''
-    '''
+    """
+    """
+
     @property
     def gravity(self):
-        '''位置属性
-        '''
+        """位置属性
+        """
         return Gravity(self._driver.get_control_gravity(self.hashcode))
 
+
 class ProgressBar(View):
-    '''进度条
-    '''
+    """进度条
+    """
+
     @property
     def progress(self):
-        '''进度
-        '''
+        """进度
+        """
         return self._driver.get_control_progress(self.hashcode)
 
+
 class SeekBar(ProgressBar):
-    '''可修改进度的进度条
-    '''
+    """可修改进度的进度条
+    """
+
     @property
     def progress(self):
-        '''进度
-        '''
+        """进度
+        """
         return super(SeekBar, self).progress
-    
+
     @progress.setter
     def progress(self, new_progress):
-        '''设置新的进度
+        """设置新的进度
         
         :param new_progress: 新进度值,取值范围:0-100
         :type new_progress:  float
-        '''
+        """
         timeout = 10
         time0 = time.time()
         while time.time() - time0 < timeout:
             rect = self.rect
             if rect[2] == 0 or rect[3] == 0:
                 time.sleep(0.2)
                 continue
             break
         offset_y = rect[3] // 2
         offset_x = rect[2] * new_progress / 100.0
         self.click(offset_x, offset_y)
-        
+
+
 class ScrollView(FrameLayout):
-    '''滚动视图
-    '''
+    """滚动视图
+    """
 
     @property
     def reach_top(self):
-        '''滑动区域达到顶部
-        '''
+        """滑动区域达到顶部
+        """
         scroll_rect = self._driver.get_control_scroll_rect(self.hashcode)
         return scroll_rect[1] == 0
 
     @property
     def reach_bottom(self):
-        '''滑动区域达到底部
-        '''
+        """滑动区域达到底部
+        """
         scroll_rect = self._driver.get_control_scroll_rect(self.hashcode)
         return scroll_rect[1] + scroll_rect[3] >= scroll_rect[5]
-    
+
     def _scroll(self, x, y, count=5, interval=0.04):
-        '''横向或纵向滚动
+        """横向或纵向滚动
         
         :param x: x > 0 时向左滑动，x = x1 - x2，滚动条向右
         :type x:  int
         :param y: y > 0 时向上滑动，y = y1 - y2，滚动条向下
         :type y:  int
         :param    count: 分为几次滑动
         :type     count:  int
-        '''
-        if y != 0: y = y * 100 // abs(y) if abs(y) < 100 else y  # 为防止在某个控件内滚动变成点击,设置最小滑动距离为100
+        """
+        if y != 0:
+            y = y * 100 // abs(y) if abs(y) < 100 else y  # 为防止在某个控件内滚动变成点击,设置最小滑动距离为100
         rect = self.rect
-        
+
         mid_x = rect[0] + rect[2] // 2  # 中点
         mid_y = rect[1] + rect[3] // 2
-        
+
         interval *= 1000  # 秒转换成毫秒
         if x != 0:
             x1 = mid_x + x // 2
             x2 = mid_x - x // 2
         else:
             x1 = x2 = mid_x
-        
+
         if y != 0:
             y1 = mid_y + y // 2
             y2 = mid_y - y // 2
         else:
             y1 = y2 = mid_y
-            
+
         self._driver.drag(x1, y1, x2, y2, count, interval)
-        
+
     def scroll(self, x, y, count=5, interval=0.04):
-        '''横向或纵向滚动
+        """横向或纵向滚动
         
         :param x: x > 0 时向左滑动，x = x1 - x2，滚动条向右
         :type x:  int
         :param y: y > 0时向上滑动，y = y1 - y2，滚动条向下
         :type y:  int
         :param    count: 分为几次滑动
         :type     count:  int
-        '''
+        """
         # 为避免在不可滑动区域滑动，每次滑动只在可滑动区域3/4处滑动
         time0 = time.time()
         while time.time() - time0 < 10:
             rect = self.rect
             if rect[2] == 0 or rect[3] == 0:
                 time.sleep(0.5)
             else:
                 break
-            
+
         max_x = rect[2] * 3 // 4
         max_y = rect[3] * 3 // 4
-        
+
         while abs(x) >= max_x:
             self._scroll(max_x * x // abs(x), 0)
             x -= max_x * x // abs(x)
-        if x != 0:self._scroll(x, 0)
-        
+        if x != 0:
+            self._scroll(x, 0)
+
         while abs(y) >= max_y:
             self._scroll(0, max_y * y // abs(y))
             y -= max_y * y // abs(y)
-        if y != 0:self._scroll(0, y)
-        
+        if y != 0:
+            self._scroll(0, y)
+
     def on_scroll(self, x, y):
         time.sleep(0.5)
 
     def scroll_up_one_page(self):
-        '''向上滑动一页
-        '''
-        if self.reach_top: return False
+        """向上滑动一页
+        """
+        if self.reach_top:
+            return False
         rect = self.rect
         scroll_y = rect[3]
-#        scroll_rect = self.driver.get_control_scroll_rect(self.hashcode)
-#        if scroll_y > scroll_rect[1]:
-#            scroll_y = scroll_rect[1]
+        #        scroll_rect = self.driver.get_control_scroll_rect(self.hashcode)
+        #        if scroll_y > scroll_rect[1]:
+        #            scroll_y = scroll_rect[1]
         self.scroll(0, -scroll_y)
         self.on_scroll(0, -scroll_y)
         return True
 
     def scroll_down_one_page(self):
-        '''向下滑动一页
-        '''
-        if self.reach_bottom: return False
+        """向下滑动一页
+        """
+        if self.reach_bottom:
+            return False
         rect = self.rect
         scroll_y = rect[3]
-#        scroll_rect = self.driver.get_control_scroll_rect(self.hashcode)
-#        offset = scroll_rect[5] - scroll_rect[1] + scroll_rect[3]
-#        if scroll_y > offset:
-#            scroll_y = offset
+        #        scroll_rect = self.driver.get_control_scroll_rect(self.hashcode)
+        #        offset = scroll_rect[5] - scroll_rect[1] + scroll_rect[3]
+        #        if scroll_y > offset:
+        #            scroll_y = offset
         self.scroll(0, scroll_y)
         self.on_scroll(0, scroll_y)
         return True
 
     def scroll_to_top(self):
-        '''滑动到顶部
-        '''
-        if self.reach_top: return
+        """滑动到顶部
+        """
+        if self.reach_top:
+            return
         rect = self.rect
         while not self.reach_top:
             self.scroll(0, -rect[3])
             self.on_scroll(0, -rect[3])
         self._wait_for_refresh_complete()  # 可能会出现刷新操作
 
     def scroll_to_bottom(self):
-        '''滑动到底部
-        '''
-        if self.reach_bottom: return
+        """滑动到底部
+        """
+        if self.reach_bottom:
+            return
         rect = self.rect
         while not self.reach_bottom:
             self.scroll(0, rect[3])
             self.on_scroll(0, rect[3])
 
     def _wait_for_refresh_complete(self, timeout=20):
-        '''等待刷新完成
-        '''
+        """等待刷新完成
+        """
         outer_top = self.rect[1]
         if len(self.children) > 0:
             time0 = time.time()
             while time.time() - time0 < timeout:
                 children = self.children
                 if len(children) > 0:  # 没有子节点时等待
                     try:
                         inner_top = children[0].rect[1]
                     except RuntimeError as e:
-                        logger.warn('_wait_for_refresh_complete error: %s' % e)
+                        logger.warn("_wait_for_refresh_complete error: %s" % e)
                         time.sleep(0.5)
                         continue
-                    if inner_top <= outer_top: return True
+                    if inner_top <= outer_top:
+                        return True
                 time.sleep(0.5)
         return False
 
     def pull_down_refresh(self):
-        '''下拉刷新
-        '''
+        """下拉刷新
+        """
         rect = self.rect
         while rect[2] == 0 or rect[3] == 0:
             time.sleep(0.1)
             rect = self.rect
         self.scroll_to_top()
         # self.scroll(0, -rect[3], 10, 0.1)  # 通过增加滑动次数增加时间，一般下拉时需要暂停一下才会触发刷新操作
         x = rect[0] + rect[2] // 2
         y1 = rect[1] + rect[3] // 4
         y2 = rect[1] + rect[3] * 3 // 4
-        
+
         self._driver.drag(x, y1, x, y2, send_down_event=True, send_up_event=False)
         time.sleep(1)  # 按住不动
         self._driver.drag(x, y2, x, y2, send_down_event=False, send_up_event=True)
-        
+
         self._wait_for_refresh_complete()
         time.sleep(1.5)  # 有些控件刷新完立即操作会不成功
-        
+
+
 class AbsListView(ScrollView):
-    '''ListView和GridView基类
-    '''
+    """ListView和GridView基类
+    """
+
     def __init__(self, *args, **kwds):
         super(AbsListView, self).__init__(*args, **kwds)
         self._first_visible_position = 0  # 可见的第一个控件索引
         self._last_visible_position = 0  # 可见的最后一个索引
         self._item_count = 0  # 所有子节点个数
         self._children = []
         self._first_update = True  # 第一次更新时需要多做些操作
 
     def __iter__(self):
-        '''迭代器
-        '''
+        """迭代器
+        """
         self.update()
         for i in range(self.item_count):
             if i < self.first_position:
                 # 需要往上滑动
                 while i < self.first_position:
                     self.scroll_up_one_page()
                 if i > self.last_position:  # 防止滚过
                     self.scroll(0, 100 * (i - self.last_position + 1))
                     self.update()
             elif i > self.last_position:
                 # 需要往下滑动
                 while i > self.last_position:
-                    if i >= self.item_count: return
+                    if i >= self.item_count:
+                        return
                     self.scroll_down_one_page()
                 if i < self.first_position:
                     self.scroll(0, -100 * (self.first_position - i + 1))
                     self.update()
 
             idx = i - self.first_position
             if idx >= len(self._children):
                 # 可能之前拉到的数据不正确
                 self.update()
             if idx < 0 or idx >= len(self._children):
-                raise IndexError('%d 不在范围[0, %d]中' % (idx, len(self._children) - 1))
+                raise IndexError("%d 不在范围[0, %d]中" % (idx, len(self._children) - 1))
             yield ListItem(self._children[idx])
 
     def __len__(self):
         self.update()
         return self.item_count
 
     def __getitem__(self, key):
-        '''支持listview[i]方式访问子控件
-        '''
+        """支持listview[i]方式访问子控件
+        """
         if isinstance(key, int):
             return self.get_child(key)
         else:
-            raise TypeError('只支持整型索引')
+            raise TypeError("只支持整型索引")
 
     def __str__(self):
-        return '<%s(Count=%d) at 0x%X>' % (self.__class__.__name__, len(self), id(self))
+        return "<%s(Count=%d) at 0x%X>" % (self.__class__.__name__, len(self), id(self))
 
     @property
     def item_count(self):
         return self._item_count
 
     @property
     def first_position(self):
@@ -1474,690 +1663,791 @@
         self.update()
         if self.reach_top:
             self._wait_for_refresh_complete()
 
     @func_wrap
     def _update_list(self):
         listview_info = self._driver.get_listview_info(self.hashcode)
-        self._item_count = listview_info['Count']
-        self._first_visible_position = listview_info['FirstPosition']
-        self._last_visible_position = listview_info['LastPosition']
+        self._item_count = listview_info["Count"]
+        self._first_visible_position = listview_info["FirstPosition"]
+        self._last_visible_position = listview_info["LastPosition"]
         if self._item_count > 0:
             self._children = self.children  # 防止每次都访问
 
     def update(self):
         for _ in range(20):
             show_count = self._last_visible_position - self._first_visible_position + 1
             self._update_list()
-            if self._first_visible_position >= 0 and self._last_visible_position >= 0 and len(self._children) == self._last_visible_position - self._first_visible_position + 1:
+            if (
+                self._first_visible_position >= 0
+                and self._last_visible_position >= 0
+                and len(self._children)
+                == self._last_visible_position - self._first_visible_position + 1
+            ):
                 # 防止控件树还在构建过程
                 if not self._first_update:
-                    show_count_now = self._last_visible_position - self._first_visible_position + 1
-                    if show_count_now == show_count: return  # 刷新前后显示的节点数目不变才是稳定状态
+                    show_count_now = (
+                        self._last_visible_position - self._first_visible_position + 1
+                    )
+                    if show_count_now == show_count:
+                        return  # 刷新前后显示的节点数目不变才是稳定状态
                 self.wait_for_complete()
                 self._first_update = False
                 return
             time.sleep(0.1)
 
     def get_child(self, idx):
-        '''提供使用索引访问子元素的方法
-        '''
+        """提供使用索引访问子元素的方法
+        """
         self.update()
         item_count = self.item_count
         if idx < 0:
             # 允许使用负数索引
             idx += item_count
         if idx < 0 or idx >= item_count:
-            raise IndexError('index=%d超出list范围' % idx)
+            raise IndexError("index=%d超出list范围" % idx)
         if idx < self.first_position:
             # 需要往上滑动
             while idx < self.first_position:
                 self.scroll_up_one_page()
         elif idx > self.last_position:
             # 需要往下滑动
             while idx > self.last_position:
                 self.scroll_down_one_page()
         idx = idx - self.first_position
         if idx < 0 or idx >= len(self._children):
-            raise IndexError('index=%d错误，不在范围[0, %d]中' % (idx, len(self._children) - 1))
+            raise IndexError("index=%d错误，不在范围[0, %d]中" % (idx, len(self._children) - 1))
         return ListItem(self._children[idx], idx)
-    
+
     @property
     def reach_top(self):
         return self.reached_top
-    
+
     @property
     def reached_top(self):
-        '''滑动区域达到顶部
-        '''
+        """滑动区域达到顶部
+        """
         for _ in range(3):
             self.update()
-            if self.first_position > 0: return False
-            if self.item_count == 0: return True
-            if len(self._children) == 0: return True
+            if self.first_position > 0:
+                return False
+            if self.item_count == 0:
+                return True
+            if len(self._children) == 0:
+                return True
             # 此时第一个子节点肯定可见
             rect = View.rect.fget(self)  # 子类可能会重载rect以修改滑动范围，此时不能根据子类的实现来计算
             try:
                 crect = self._children[0].rect
             except RuntimeError as e:
                 from qt4a.androiddriver.util import logger
+
                 # logger.warn('reach_top error: %s' % e)
                 logger.exception(e)
                 continue
             return crect[1] >= rect[1]
-    
+
     @property
     def reach_bottom(self):
         return self.reached_bottom
-    
+
     @property
     def reached_bottom(self):
-        '''滑动区域达到底部
-        '''
-        if self.item_count == 0: self.update()
+        """滑动区域达到底部
+        """
+        if self.item_count == 0:
+            self.update()
         return self.last_position == self.item_count - 1
 
-#    def scroll_to_top(self):
-#        '''滑动到顶部
-#        '''
-#        if self.reach_top: return
-#        rect = self.bounding_rect
-#        scroll_total = 0
-#        while not self.reach_top:
-#            scroll_y = self.first_position * 100  # 以每一项100的高度计算
-#            if scroll_y > rect[3]: scroll_y = rect[3]
-#            print ('scroll', -scroll_y)
-#            self.scroll(0, -scroll_y)
-#            scroll_total += scroll_y
-#        self.on_scroll(0, -scroll_total)
-#    
+    #    def scroll_to_top(self):
+    #        '''滑动到顶部
+    #        '''
+    #        if self.reach_top: return
+    #        rect = self.bounding_rect
+    #        scroll_total = 0
+    #        while not self.reach_top:
+    #            scroll_y = self.first_position * 100  # 以每一项100的高度计算
+    #            if scroll_y > rect[3]: scroll_y = rect[3]
+    #            print ('scroll', -scroll_y)
+    #            self.scroll(0, -scroll_y)
+    #            scroll_total += scroll_y
+    #        self.on_scroll(0, -scroll_total)
+    #
     def scroll_up_one_page(self):
-        '''向上滑动一页
-        '''
-        if self.reached_top: return False
+        """向上滑动一页
+        """
+        if self.reached_top:
+            return False
         rect = self.rect
         scroll_y = rect[3]
         if scroll_y > self.first_position * 100:
             scroll_y = self.first_position * 100
-        if scroll_y < 100: scroll_y = 100
+        if scroll_y < 100:
+            scroll_y = 100
         self.scroll(0, -scroll_y)
         self.on_scroll(0, -scroll_y)
         return True
 
     def scroll_down_one_page(self):
-        '''向下滑动一页
-        '''
-        if self.reached_bottom: return False
+        """向下滑动一页
+        """
+        if self.reached_bottom:
+            return False
         rect = self.rect
         scroll_y = rect[3]
         offset = (self.item_count - self.last_position) * 100
         if scroll_y > offset:
             scroll_y = offset
         self.scroll(0, scroll_y)
         self.on_scroll(0, scroll_y)
         return True
 
     def wait_for_complete(self, timeout=2):
-        '''等待ListView控件变化，比如需要读取本地数据
-        '''
+        """等待ListView控件变化，比如需要读取本地数据
+        """
         count0 = self.item_count
         first_position0 = self.first_position
         last_position0 = self.last_position
 
         time0 = time.time()
         while time.time() - time0 < timeout:
             time.sleep(0.2)
             self._update_list()
-            if self._first_visible_position >= 0 and self._last_visible_position >= 0 and len(self._children) == self._last_visible_position - self._first_visible_position + 1:
+            if (
+                self._first_visible_position >= 0
+                and self._last_visible_position >= 0
+                and len(self._children)
+                == self._last_visible_position - self._first_visible_position + 1
+            ):
                 count = self.item_count
                 first_position = self.first_position
                 last_position = self.last_position
-                if count == count0 and first_position == first_position0 and last_position == last_position0: return True
+                if (
+                    count == count0
+                    and first_position == first_position0
+                    and last_position == last_position0
+                ):
+                    return True
                 count0 = count
                 first_position0 = first_position
                 last_position0 = last_position
         return False
 
+
 class ListItem(View):
-    '''为方便遍历AbsListView，表示AbsListView的直接子孩子
-    '''
+    """为方便遍历AbsListView，表示AbsListView的直接子孩子
+    """
+
     def __init__(self, view, idx=None):
-        '''
+        """
         :param view: AbsListView中每一个子节点
         :type view:  View
-        '''
+        """
         self._view = view
         self._control_dict = {}  # 用于缓存
         self._idx = idx  # 项索引，用于重新查找控件
-        
+
     def __getitem__(self, key):
-        '''支持listitem[key]方式访问子节点
+        """支持listitem[key]方式访问子节点
         :param key: 封装时定义的子节点名
         :type key:  string
-        '''
+        """
         if key in self._control_dict:
             return self._control_dict[key]
         item = self._view.container[key]
         import copy
+
         result = copy.copy(item)  # 复制一个对象
         result._root = self  # 修改根节点为当前节点
         self._control_dict[key] = result
         return result
 
     def __getattr__(self, attr):
-        '''委托self._view实现
-        '''
+        """委托self._view实现
+        """
         return getattr(self._view, attr)
-    
+
     def _update(self):
-        '''如果没有索引值直接抛异常
-        '''
+        """如果没有索引值直接抛异常
+        """
         from qt4a.androiddriver.util import logger
-        logger.debug('ListItem update, idx=%s' % self._idx)
+
+        logger.debug("ListItem update, idx=%s" % self._idx)
         if self._idx == None:
-            raise RuntimeError('ListView无法重新获取控件')
+            raise RuntimeError("ListView无法重新获取控件")
         self._view._root.update()
         self._view = self._view._root._children[self._idx]  # 重新获取Item项
-    
+
     def has(self, key):
-        '''是否存在该节点
+        """是否存在该节点
         
         :param key: 封装时定义的子节点名
         :type  key: string
-        '''
+        """
         from qt4a.androiddriver.util import ControlExpiredError, logger
+
         item = self._view.container[key]
         # child = self._driver.get_control(self._activity, self.hashcode, item._locator)
         self._view._need_convert_qpath = True  # 避免判断多个节点存在时不会使用整型ID查找问题
         try:
             hashcode = self._view._get_hashcode(self._view.hashcode, item._locator)
-            if hashcode == 0: return False
+            if hashcode == 0:
+                return False
         except ControlExpiredError:
-            logger.info('ControlExpiredError occur in has')
-            if self._idx == None: return False
+            logger.info("ControlExpiredError occur in has")
+            if self._idx == None:
+                return False
             self._update()
             return self.has(key)
         item._locator = self._locator  # 替换为真正的QPath
         return True
 
+
 class ListView(AbsListView):
-    '''列表视图
-    '''
+    """列表视图
+    """
+
     pass
 
+
 class GridView(AbsListView):
-    '''格子视图
-    '''
+    """格子视图
+    """
+
 
 class TabWidget(View):
-    '''Tab控件
-    '''
+    """Tab控件
+    """
+
     @property
     def selected_index(self):
-        '''当前所选项的索引
-        '''
+        """当前所选项的索引
+        """
         return self._driver.get_selected_tab_index(self.hashcode)
 
+
 class WebkitWebView(View):
-    '''4.4以下版本中的WebView
-    '''
-    
+    """4.4以下版本中的WebView
+    """
+
     def __init__(self, *args, **kwargs):
         super(WebkitWebView, self).__init__(*args, **kwargs)
-    
+
     def eval_script(self, frame_xpaths, script):
-        '''执行JavaScript
-        '''
+        """执行JavaScript
+        """
         from qt4a.androiddriver.util import AndroidSpyError, ControlExpiredError
+
         try:
             return self._driver.eval_script(self.hashcode, frame_xpaths, script)
         except ControlExpiredError as e:
             raise e
         except AndroidSpyError as e:
             try:
                 from qt4w.util import JavaScriptError
             except ImportError:
                 raise
             else:
                 raise JavaScriptError(frame_xpaths, e.args[0])
-            
+
+
 class WebView(View):
-    '''Web页面容器
-    '''
+    """Web页面容器
+    """
+
     title = None
     url = None
     is_chromium = None
-    
+
     def __init__(self, *args, **kwargs):
         self._args = args
         self._kwargs = kwargs
         super(WebView, self).__init__(*args, **kwargs)
         self._is_chromium = self.__class__.is_chromium
-        if self._is_chromium == None: self._is_chromium = self.container.device.sdk_version >= 19  # Android 4.4以上使用Chromium内核
+        if self._is_chromium == None:
+            self._is_chromium = (
+                self.container.device.sdk_version >= 19
+            )  # Android 4.4以上使用Chromium内核
         self._webview_impl = None
-    
+
     @property
     def webdriver_class(self):
-        '''WebView对应的WebDriver类
-        '''
+        """WebView对应的WebDriver类
+        """
         from qt4a.androiddriver.webdriver import AndroidWebDriver
+
         return AndroidWebDriver
-    
+
     @property
     def webview_impl(self):
-        '''
-        '''
+        """
+        """
         if self._webview_impl == None:
             if not self._is_chromium:
                 self._webview_impl = WebkitWebView(*self._args, **self._kwargs)
             else:
                 try:
-                    self._webview_impl = ChromiumWebView(title=self.__class__.title, url=self.__class__.url, *self._args, **self._kwargs)
+                    self._webview_impl = ChromiumWebView(
+                        title=self.__class__.title,
+                        url=self.__class__.url,
+                        *self._args,
+                        **self._kwargs
+                    )
                 except ImportError:
                     # Fallback to custom WebView
                     self._webview_impl = WebkitWebView(*self._args, **self._kwargs)
 
         return self._webview_impl
-    
+
     def eval_script(self, frame_xpaths, script):
-        '''在指定frame中执行JavaScript，并返回执行结果（该实现需要处理js基础库未注入情况的处理）
+        """在指定frame中执行JavaScript，并返回执行结果（该实现需要处理js基础库未注入情况的处理）
         
         :param frame_xpaths: frame元素的XPATH路径，如果是顶层页面，怎传入“[]”
         :type frame_xpaths:  list
         :param script:       要执行的JavaScript语句
         :type script:        string
-        '''
+        """
         return self.webview_impl.eval_script(frame_xpaths, script)
-    
+
     @property
     def visible_rect(self):
-        '''WebView控件可见区域的坐标信息
-        '''
+        """WebView控件可见区域的坐标信息
+        """
         return self.rect
-            
+
     def disable_soft_input(self):
-        '''禁用软键盘
-        '''
+        """禁用软键盘
+        """
         return self._driver.enable_soft_input(self.hashcode, False)
-    
+
     def click(self, x_offset=None, y_offset=None):
-        '''点击WebView中的某个坐标
+        """点击WebView中的某个坐标
         
         :param x_offset: 与WebView左上角的横向偏移量
         :type x_offset:  int/float
         :param y_offset: 与WebView左上角的纵向偏移量
         :type y_offset:  int/float
-        '''
+        """
         if x_offset != None or y_offset != None:
             rect = self.rect
             x = (rect[0] + rect[2] // 2) if not x_offset else (rect[0] + x_offset)
             y = (rect[1] + rect[3] // 2) if not y_offset else (rect[1] + y_offset)
             return self._click(0, x, y)
         else:
             return super(WebView, self).click()
-    
+
     def long_click(self, x_offset, y_offset, duration=1):
-        '''长按WebView中的某个坐标
+        """长按WebView中的某个坐标
         
         :param x_offset: 与WebView左上角的横向偏移量
         :type x_offset:  int/float
         :param y_offset: 与WebView左上角的纵向偏移量
         :type y_offset:  int/float
         :param duration: 按住的持续时间
         :type duration:  int/float
-        '''
+        """
         return super(WebView, self).long_click(duration, x_offset, y_offset)
-    
+
     def send_keys(self, keys):
-        '''向WebView中的输入框发送按键
+        """向WebView中的输入框发送按键
         
         :param keys: 要发送的按键
         :type keys:  string
-        '''
+        """
         self.container.device.send_text(keys)
-        #self._driver.send_keys(keys)
-    
+        # self._driver.send_keys(keys)
+
     def drag(self, x1, y1, x2, y2):
-        '''从(x1, y1)点滑动到(x2, y2)点
+        """从(x1, y1)点滑动到(x2, y2)点
         
         :param x1: 起点横坐标
         :type x1:  int/float
         :param y1: 起点纵坐标
         :type y1:  int/float
         :param x2: 终点横坐标
         :type x2:  int/float
         :param y2: 终点纵坐标
         :type y2:  int/float
-        '''
+        """
         self._driver.drag(x1, y1, x2, y2, 10, 0.1)
-    
+
     def screenshot(self):
-        '''当前WebView的截图
+        """当前WebView的截图
         :return: PIL.Image
-        '''
+        """
         from PIL import Image
-        temp_path = tempfile.mktemp('.jpg')
+
+        temp_path = tempfile.mktemp(".jpg")
         self.container.device.take_screen_shot(temp_path)
-        with open(temp_path, 'rb') as fp:
+        with open(temp_path, "rb") as fp:
             image_data = fp.read()
         os.remove(temp_path)
         image = Image.open(io.BytesIO(image_data))
         left, top, width, height = self.rect
         image = image.crop((left, top, left + width, top + height))
         return image
 
 
 class ChromiumWebView(WebkitWebView):
-    '''Chromium内核的WebView
-    '''
+    """Chromium内核的WebView
+    """
+
     debugger_instances = {}
-    
+
     def __init__(self, url=None, title=None, *args, **kwargs):
         import chrome_master
+
         super(ChromiumWebView, self).__init__(*args, **kwargs)
         self._is_system_webview = False
         webview_types = self._driver.get_control_type(self.hashcode)
         for webview_type in webview_types:
-            if webview_type == 'android.webkit.WebView':
+            if webview_type == "android.webkit.WebView":
                 self._is_system_webview = True
                 break
         self._url = url
         self._title = title
-        
+
         self._device = self.container.device
         self._pid = self._device.adb.get_pid(self._driver._process_name)
-        self._service_name = 'webview_devtools_remote_%d' % self._pid
 
         chrome_master.set_logger(logger)
 
-        self._chrome_master = chrome_master.ChromeMaster(('localhost', self._pid), self.create_socket)  # 高版本Chromium内核必须要使用localhost的Host
+        self._chrome_master = chrome_master.ChromeMaster(
+            ("localhost", self._pid), self.create_socket
+        )  # 高版本Chromium内核必须要使用localhost的Host
 
         self._page_debugger = self.get_debugger()
         self._page_debugger.register_handler(chrome_master.RuntimeHandler)
 
+    def get_service_name(self):
+        return "webview_devtools_remote_%d" % self._pid
+
     def create_socket(self):
-        '''创建socket对象
-        '''
+        """创建socket对象
+        """
         try:
-            sock = self._device.adb.create_tunnel(self._service_name, 'localabstract')
-            if sock: return sock
+            sock = self._device.adb.create_tunnel(
+                self.get_service_name(), "localabstract"
+            )
+            if sock:
+                return sock
         except:
-            logger.warn('create socket tunnel %s failed' % self._service_name)
+            logger.warn("create socket tunnel %s failed" % self.get_service_name())
         self._driver.set_webview_debugging_enabled(self.hashcode, True)
         return self.create_socket()
-        
+
     def get_page_url(self):
-        '''获取当前WebView页面的url
-        '''
-        if not self._is_system_webview: return self._url
+        """获取当前WebView页面的url
+        """
+        if not self._is_system_webview:
+            return self._url
         timeout = 10
         time0 = time.time()
         while time.time() - time0 < timeout:
             try:
-                ret = super(ChromiumWebView, self).eval_script([], 'location.href')
+                ret = super(ChromiumWebView, self).eval_script([], "location.href")
             except:
-                logger.exception('Read page url failed')
+                logger.exception("Read page url failed")
                 return
-            if ret != 'about:blank': return ret
+            if ret != "about:blank":
+                return ret
             time.sleep(0.5)
         else:
-            raise RuntimeError('Get page url failed')
-    
+            raise RuntimeError("Get page url failed")
+
     def get_debugger(self, timeout=10):
-        '''获取当前页面的RemoteDebugger实例
-        '''
+        """获取当前页面的RemoteDebugger实例
+        """
         url = self.get_page_url()
         time0 = time.time()
         while time.time() - time0 < timeout:
             try:
-                return self._chrome_master.find_page(url=url, title=self._title)  # 获取最后一个页面
+                return self._chrome_master.find_page(
+                    url=url, title=self._title
+                )  # 获取最后一个页面
             except RuntimeError as e:
-                logger.warn('[%s] %s' % (self.__class__.__name__, e))
+                logger.warn("[%s] %s" % (self.__class__.__name__, e))
                 time.sleep(0.5)
         else:
-            raise RuntimeError('Find page timeout')
+            raise RuntimeError("Find page timeout")
 
     def convert_frame_tree(self, frame_tree, parent=None):
-        '''将frame tree转化为Frame对象
-        '''
+        """将frame tree转化为Frame对象
+        """
         from qt4w import util
-        frame = util.Frame(frame_tree['frame']['id'], frame_tree['frame'].get('name'), frame_tree['frame']['url'])
-        if parent: parent.add_child(frame)
-        if 'childFrames' in frame_tree:
-            for child in frame_tree['childFrames']:
+
+        frame = util.Frame(
+            frame_tree["frame"]["id"],
+            frame_tree["frame"].get("name"),
+            frame_tree["frame"]["url"],
+        )
+        if parent:
+            parent.add_child(frame)
+        if "childFrames" in frame_tree:
+            for child in frame_tree["childFrames"]:
                 self.convert_frame_tree(child, frame)
         return frame
-        
+
     def _get_frame_id_by_xpath(self, frame_xpaths, timeout=10):
-        '''获取frame id
-        '''
+        """获取frame id
+        """
         from qt4a.androiddriver.webdriver import AndroidWebDriver
         from qt4w import util
+
         time0 = time.time()
         while time.time() - time0 < timeout:
             frame_tree = self._page_debugger.page.get_frame_tree()
             frame = self.convert_frame_tree(frame_tree)
             frame_selector = util.FrameSelector(AndroidWebDriver(self), frame)
             try:
                 frame = frame_selector.get_frame_by_xpath(frame_xpaths)
             except util.ControlNotFoundError:
                 pass
             else:
                 return frame.id
             time.sleep(0.5)
         else:
-            raise ControlNotFoundError('Find frame %s timeout' % ''.join(frame_xpaths))
-        
+            raise ControlNotFoundError("Find frame %s timeout" % "".join(frame_xpaths))
+
     def eval_script(self, frame_xpaths, script):
-        '''在指定frame中执行JavaScript，并返回执行结果
+        """在指定frame中执行JavaScript，并返回执行结果
         
         :param frame_xpaths: frame元素的XPATH路径，如果是顶层页面，怎传入“[]”
         :type frame_xpaths:  list
         :param script:       要执行的JavaScript语句
         :type script:        string
-        '''
+        """
         from chrome_master import util
+
         frame_id = None
         if frame_xpaths:
             frame_id = self._get_frame_id_by_xpath(frame_xpaths)
         for _ in range(3):
             try:
                 return self._page_debugger.runtime.eval_script(frame_id, script)
             except util.ConnectionClosedError as e:
                 self._page_debugger = self.get_debugger()
             except util.JavaScriptError as e:
                 from qt4w.util import JavaScriptError
+
                 raise JavaScriptError(frame_xpaths, e.message)
         else:
             raise util.ConnectionClosedError("Connection Closed")
-        
+
+
 class ViewPager(ViewGroup):
-    '''横向滚动视图
-    '''
+    """横向滚动视图
+    """
+
     @property
     def current_item_index(self):
-        '''当前显示项的索引
-        '''
-        ret = self._driver.get_object_field_value(self.hashcode, 'mCurItem')
+        """当前显示项的索引
+        """
+        ret = self._driver.get_object_field_value(self.hashcode, "mCurItem")
         return int(ret)
-    
+
     @property
     def item_count(self):
-        '''总项数
-        '''
-        ret = self._driver.get_object_field_value(self.hashcode, 'mItems.size')
+        """总项数
+        """
+        ret = self._driver.get_object_field_value(self.hashcode, "mItems.size")
         return int(ret)
-    
+
     def scroll(self, count=1, rect=None):
-        '''左右滚动
+        """左右滚动
         
         :param count: 滑动次数，大于0表示向右滑动，小于0表示向左滑动
         :type  count: int
-        '''
-        if rect == None: rect = self.rect
+        """
+        if rect == None:
+            rect = self.rect
         x1 = rect[0] + 5
         x2 = rect[0] + rect[2] - 5
         if count > 0:
             # 交换终点
             x = x1
             x1 = x2
             x2 = x
         y = rect[1] + rect[3] // 2
         for _ in range(abs(count)):
             self._driver.drag(x1, y, x2, y, 1)
-    
+
     def __iter__(self):
-        '''迭代器
-        '''
+        """迭代器
+        """
         for i in range(self.item_count):
             idx = self.current_item_index
             if idx > i:
                 # 向右滑动
                 self.scroll(i - idx)
             elif idx < i:
                 # 向左滑动
                 self.scroll(idx - i)
             yield ListItem(self.children[i])
-            
+
+
 class RadioGroup(LinearLayout):
-    '''
-    '''
+    """
+    """
+
     pass
 
+
 class RecyclerView(AbsListView):
-    '''虽然不是继承自ListView，但是可以复用其部分代码，所以从ListView继承过来
-    '''
+    """虽然不是继承自ListView，但是可以复用其部分代码，所以从ListView继承过来
+    """
+
     @func_wrap
     def _update_list(self):
-        self._item_count = self._driver.call_object_method(self.hashcode, 'mAdapter', 'getItemCount')
+        self._item_count = self._driver.call_object_method(
+            self.hashcode, "mAdapter", "getItemCount"
+        )
         self._first_visible_position = -1
         self._last_visible_position = -1
         if self._item_count > 0:
             self._children = self.children  # 防止每次都访问
         if len(self._children) > 0:
             # 获取第一个子节点的索引值
             self._first_visible_position = self._get_first_visible_position()
-            self._last_visible_position = self._first_visible_position + len(self._children) - 1
-    
+            self._last_visible_position = (
+                self._first_visible_position + len(self._children) - 1
+            )
+
     def _get_first_visible_position(self):
-        '''获取第一个可见节点的位置
+        """获取第一个可见节点的位置
         ('mLayoutParams', 'getViewLayoutPosition')
-        '''
-        if hasattr(self, '_get_first_visible_position_args'):
-            return self._driver.call_object_method(self._children[0].hashcode, *self._get_first_visible_position_args)
-        
-        for args in (('mLayoutParams.mViewHolder', 'getPosition'),
-                     ('mLayoutParams.mViewHolder', 'getLayoutPosition')):
+        """
+        if hasattr(self, "_get_first_visible_position_args"):
+            return self._driver.call_object_method(
+                self._children[0].hashcode, *self._get_first_visible_position_args
+            )
+
+        for args in (
+            ("mLayoutParams.mViewHolder", "getPosition"),
+            ("mLayoutParams.mViewHolder", "getLayoutPosition"),
+        ):
             try:
-                result = self._driver.call_object_method(self._children[0].hashcode, *args)
+                result = self._driver.call_object_method(
+                    self._children[0].hashcode, *args
+                )
                 self._get_first_visible_position_args = args
                 return result
             except:
-                logger.exception('get first visible position by %r failed' % args)
-        
+                logger.exception("get first visible position by %r failed" % args)
+
     def _is_horizontal(self):
-        '''是否横向滑动
-        '''
-        if not hasattr(self, '__horizontal'):
+        """是否横向滑动
+        """
+        if not hasattr(self, "__horizontal"):
             if self.item_count >= 2:
                 self.__horizontal = self.children[0].rect[0] != self.children[1].rect[0]
             elif self.item_count == 1:
                 x_ratio = 1.0 * self.children[0].rect[2] / self.rect[2]
                 y_ratio = 1.0 * self.children[0].rect[3] / self.rect[3]
                 self.__horizontal = x_ratio < y_ratio
             else:
                 return False
         return self.__horizontal
-    
+
     @property
     def reached_left(self):
-        '''滑动区域达到最左边
-        '''
+        """滑动区域达到最左边
+        """
         for _ in range(3):
             self.update()
-            if self.first_position > 0: return False
-            if self.item_count == 0: return True
-            if len(self._children) == 0: return True
+            if self.first_position > 0:
+                return False
+            if self.item_count == 0:
+                return True
+            if len(self._children) == 0:
+                return True
             # 此时第一个子节点肯定可见
             rect = View.rect.fget(self)  # 子类可能会重载rect以修改滑动范围，此时不能根据子类的实现来计算
             try:
                 crect = self._children[0].rect
             except RuntimeError as e:
                 logger.exception(e)
                 continue
             return crect[0] >= rect[0]
 
     @property
     def reached_right(self):
-        '''滑动区域达到最右边
-        '''
-        if self.item_count == 0: self.update()
+        """滑动区域达到最右边
+        """
+        if self.item_count == 0:
+            self.update()
         return self.last_position == self.item_count - 1
-        
+
     def scroll_left_one_page(self):
-        '''向左滑动一页
-        '''
-        if self.reached_left: return False
+        """向左滑动一页
+        """
+        if self.reached_left:
+            return False
         rect = self.rect
         scroll_x = rect[2]
         item_rect = self._children[0].rect
         if scroll_x > self.first_position * item_rect[2]:
             scroll_x = self.first_position * item_rect[2]
-        if scroll_x < 100: scroll_x = 100
+        if scroll_x < 100:
+            scroll_x = 100
         self.scroll(-scroll_x, 0)
         self.on_scroll(-scroll_x, 0)
         return True
 
     def scroll_right_one_page(self):
-        '''向右滑动一页
-        '''
-        if self.reached_right: return False
+        """向右滑动一页
+        """
+        if self.reached_right:
+            return False
         rect = self.rect
         scroll_x = rect[2]
         item_rect = self._children[0].rect
         offset = (self.item_count - self.last_position) * item_rect[2]
         if scroll_x > offset:
             scroll_x = offset
         self.scroll(scroll_x, 0)
         self.on_scroll(scroll_x, 0)
         return True
-    
+
     def scroll_up_one_page(self):
-        '''向上滑动一页
-        '''
-        if self.reached_top: return False
+        """向上滑动一页
+        """
+        if self.reached_top:
+            return False
         rect = self.rect
         scroll_y = rect[3]
         child_rect = self._children[0].rect
         if scroll_y > self.first_position * child_rect[3]:
             scroll_y = self.first_position * child_rect[3]
-        if scroll_y < child_rect[3]: scroll_y = child_rect[3]
+        if scroll_y < child_rect[3]:
+            scroll_y = child_rect[3]
         self.scroll(0, -scroll_y)
         self.on_scroll(0, -scroll_y)
         return True
 
     def scroll_down_one_page(self):
-        '''向下滑动一页
-        '''
-        if self.reached_bottom: return False
+        """向下滑动一页
+        """
+        if self.reached_bottom:
+            return False
         rect = self.rect
         scroll_y = rect[3]
         child_rect = self._children[0].rect
         offset = (self.item_count - self.last_position) * child_rect[3]
         if scroll_y > offset:
             scroll_y = offset
         elif scroll_y < child_rect[3]:
             scroll_y = child_rect[3]
         self.scroll(0, scroll_y)
         self.on_scroll(0, scroll_y)
         return True
-    
+
     def _scroll_child_to_visible(self, child_idx):
-        '''将子节点滚动到可见区域
-        '''
+        """将子节点滚动到可见区域
+        """
         if child_idx < self.first_position:
             # 需要往左/上滑动
             while child_idx < self.first_position:
                 if self._is_horizontal():
                     self.scroll_left_one_page()
                 else:
                     self.scroll_up_one_page()
@@ -2166,94 +2456,113 @@
             # 需要往右/下滑动
             while child_idx > self.last_position:
                 if self._is_horizontal():
                     self.scroll_right_one_page()
                 else:
                     self.scroll_down_one_page()
                 self._update_list()
-                
+
         child = self.children[child_idx - self.first_position]
         self_rect = self.rect
         child_rect = child.rect
-        
+
         # 保证当前项完全可见
-        
-        if child_rect[0] < self_rect[0]: 
+
+        if child_rect[0] < self_rect[0]:
             # 向左滑动
             scroll_x = self_rect[0] - child_rect[0]
             self.scroll(-scroll_x, 0)
-        elif child_rect[0] + child_rect[2] > self_rect[0] + self_rect[2]: 
+        elif child_rect[0] + child_rect[2] > self_rect[0] + self_rect[2]:
             # 向右滑动
             scroll_x = child_rect[0] + child_rect[2] - (self_rect[0] + self_rect[2])
             self.scroll(scroll_x, 0)
-        elif child_rect[1] < self_rect[1]: 
+        elif child_rect[1] < self_rect[1]:
             # 向上滑动
             scroll_y = self_rect[1] - child_rect[1]
             self.scroll(0, -scroll_y)
         elif child_rect[1] + child_rect[3] > self_rect[1] + self_rect[3]:
             # 向下滑动
             scroll_y = child_rect[1] + child_rect[3] - (self_rect[1] + self_rect[3])
             self.scroll(0, scroll_y)
         else:
             return
         self._update_list()
-        
+
     def get_child(self, idx):
-        '''提供使用索引访问子元素的方法
-        '''
+        """提供使用索引访问子元素的方法
+        """
         self.update()
         item_count = self.item_count
         if idx < 0:
             # 允许使用负数索引
             idx += item_count
         if idx < 0 or idx >= item_count:
-            raise IndexError('index=%d超出list范围' % idx)
+            raise IndexError("index=%d超出list范围" % idx)
         self._scroll_child_to_visible(idx)
         idx = idx - self.first_position
         if idx < 0 or idx >= len(self._children):
-            raise IndexError('index=%d错误，不在范围[0, %d]中' % (idx, len(self._children) - 1))
+            raise IndexError("index=%d错误，不在范围[0, %d]中" % (idx, len(self._children) - 1))
         return ListItem(self._children[idx], idx)
-    
+
     def __iter__(self):
-        '''迭代器
-        '''
+        """迭代器
+        """
         self.update()
         for i in range(self.item_count):
             self._scroll_child_to_visible(i)
 
             idx = i - self.first_position
             if idx >= len(self._children):
                 # 可能之前拉到的数据不正确
                 self.update()
             if idx < 0 or idx >= len(self._children):
-                raise IndexError('%d 不在范围[0, %d]中' % (idx, len(self._children) - 1))
+                raise IndexError("%d 不在范围[0, %d]中" % (idx, len(self._children) - 1))
             yield ListItem(self._children[idx])
 
+
 class DatePicker(FrameLayout):
-    '''时间选择器
-    '''
-    def set_date(self, year, month, day): 
+    """时间选择器
+    """
+
+    def set_date(self, year, month, day):
         if year < 0 or month < 1 or month > 12 or day < 1 or day > 31:
-            raise RuntimeError('参数传入不符合时间要求')
+            raise RuntimeError("参数传入不符合时间要求")
 
         if self._driver._adb.get_sdk_version() < 21:  # 5.0以下用如下方法
-            self._driver.call_object_method(self.hashcode, 'mCurrentDate', 'set', 'void', year, month - 1, day)
+            self._driver.call_object_method(
+                self.hashcode, "mCurrentDate", "set", "void", year, month - 1, day
+            )
         else:
-            self._driver.call_object_method(self.hashcode, 'mDelegate.mCurrentDate', 'set', 'void', year, month - 1, day)
+            self._driver.call_object_method(
+                self.hashcode,
+                "mDelegate.mCurrentDate",
+                "set",
+                "void",
+                year,
+                month - 1,
+                day,
+            )
+
 
 class ActionMenuItemView(TextView):
-    '''android.support.v7.internal.view.menu.ActionMenuItemView
-    '''
+    """android.support.v7.internal.view.menu.ActionMenuItemView
+    """
+
     pass
 
+
 class AppCompatEditText(EditText):
-    '''android.support.v7.widget.AppCompatEditText
-    '''
+    """android.support.v7.widget.AppCompatEditText
+    """
+
     pass
 
+
 class AppCompatImageView(ImageView):
-    '''android.support.v7.widget.AppCompatImageView
-    '''
+    """android.support.v7.widget.AppCompatImageView
+    """
+
     pass
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     pass
```

### Comparing `qt4a-2.3.1/qt4a/androidapp.py` & `qt4a-3.0.0/qt4a/androidapp.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,259 +1,288 @@
 # -*- coding: UTF-8 -*-
 #
 # Tencent is pleased to support the open source community by making QTA available.
 # Copyright (C) 2016THL A29 Limited, a Tencent company. All rights reserved.
-# Licensed under the BSD 3-Clause License (the "License"); you may not use this 
+# Licensed under the BSD 3-Clause License (the "License"); you may not use this
 # file except in compliance with the License. You may obtain a copy of the License at
-# 
+#
 # https://opensource.org/licenses/BSD-3-Clause
-# 
-# Unless required by applicable law or agreed to in writing, software distributed 
+#
+# Unless required by applicable law or agreed to in writing, software distributed
 # under the License is distributed on an "AS IS" basis, WITHOUT WARRANTIES OR CONDITIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 #
 
-'''Android App基类
-'''
+"""Android App基类
+"""
 
 
 import re
 import threading
 import time
 
 from tuia.exceptions import ControlNotFoundError
 from qt4a.androiddriver.androiddriver import AndroidDriver
 from qt4a.androiddriver.util import logger, ThreadEx, EnumThreadPriority, TimeoutError
 from qt4a.device import Device
 from qt4a.systemui import CrashWindow, AppNoResponseWindow, AppResolverPanel
 
+
 class AndroidApp(object):
-    '''Android App基类
-    '''
-    package_name = ''
+    """Android App基类
+    """
+
+    package_name = ""
 
     def __init__(self, process_name, device, init_env=True):
         self._device = device
 
         if not self.package_name:
-            raise RuntimeError('`%s.package_name` must be set' % self.__class__.__name__)
+            raise RuntimeError(
+                "`%s.package_name` must be set" % self.__class__.__name__
+            )
 
         if not self._device.is_app_installed(self.package_name):
-            raise RuntimeError('APP: %s not installed' % self.package_name)
+            raise RuntimeError("APP: %s not installed" % self.package_name)
 
         self._drivers = {}  # 如果应用存在多个被测进程，就会有多个driver
         self._process_name = process_name  # 主程序名
-        
+
         self._monitor_task_list = []
         self._monitor_run = True
-        
+
         self._app_crashed = False
         self._main_thread_id = threading.current_thread().ident  # 创建该对象的线程一定是主线程
-        
-        if not init_env: return  # 一般是调试状态
-        
+
+        if not init_env:
+            return  # 一般是调试状态
+
         self._device.unlock_keyguard()  # 解屏幕锁
         self._device.wake_screen()  # 唤醒屏幕
         self._close_other_window()
 
         self._monitor_thread = None
         self.start_monitor()
         self.add_monitor_task(self._detect_crash_window)
         if self.device.is_rooted():
             self.grant_all_runtime_permissions()
-            
+
     @property
     def device(self):
-        '''返回所在的设备
-        '''
+        """返回所在的设备
+        """
         return self._device
 
     @property
     def process_name(self):
-        '''应用所在的主进程名
-        '''
+        """应用所在的主进程名
+        """
         return self._process_name
 
     @process_name.setter
     def process_name(self, name):
         self._process_name = name
 
     @property
     def crashed(self):
         return self._app_crashed
 
     def __del__(self):
         self.close()
 
-    def get_driver(self, process_name=''):
-        '''根据进程名获取driver对象，默认为主程序driver
-        '''
+    def start_activity(self, activity_name):
+        """启动Activity"""
+        return self._device.start_activity("%s/%s" % (self.package_name, activity_name))
+
+    def clear_data(self):
+        return self._device.clear_data(self.package_name)
+
+    def get_driver(self, process_name=""):
+        """根据进程名获取driver对象，默认为主程序driver
+        """
         if not process_name:
-            if not self._process_name: raise RuntimeError('主程序名为空')
+            if not self._process_name:
+                raise RuntimeError("主程序名为空")
             process_name = self._process_name
         if not process_name in self._drivers:
             # 只有尚未创建的时候才需要互斥
             # logger.debug('wait for %s create driver' % process_name)
             # 创建driver
             driver = AndroidDriver.create(process_name, self._device)
             self._drivers[process_name] = driver
             # logger.debug('%s create driver success' % process_name)
         driver = self._drivers[process_name]
         return driver
-    
+
     def close_driver(self, process_name):
-        '''关闭测试桩
-        '''
+        """关闭测试桩
+        """
         self._drivers[process_name].close()
         del self._drivers[process_name]
-    
+
     def close_activity(self, activity):
-        '''关闭Activity
-        '''
+        """关闭Activity
+        """
         for process_name in self._drivers:
             driver = self._drivers[process_name]
             try:
                 ret = driver.close_activity(activity)
-                if ret == 0: return True
-                elif ret == -2: return False
-                logger.debug('close activity in %s return %s' % (process_name, ret))
+                if ret == 0:
+                    return True
+                elif ret == -2:
+                    return False
+                logger.debug("close activity in %s return %s" % (process_name, ret))
             except ValueError:
                 continue
         return False
-    
+
     def wait_for_activity(self, activity, timeout=15, interval=0.5):
-        '''等待Activity打开
+        """等待Activity打开
         
         :param activity: Activtiy名称
         :type activity:  string
         :param timeout:  超时时间，单位：S
         :type timeout:   int/float
         :param interval: 检查间隔时间，单位：S
         :type interval:  int/float
-        '''
+        """
         time0 = time.time()
         while time.time() - time0 < timeout:
             if self.crashed:
-                raise RuntimeError('%s Crashed' % self.__class__.__name__)
+                raise RuntimeError("%s Crashed" % self.__class__.__name__)
             current_activity = self.device.get_current_activity()
-            if current_activity == activity: return True
+            if current_activity == activity:
+                return True
             time.sleep(interval)
-        raise ControlNotFoundError('Wait for Activity %s timeout, current Activity: %s' % (activity, current_activity))
+        raise ControlNotFoundError(
+            "Wait for Activity %s timeout, current Activity: %s"
+            % (activity, current_activity)
+        )
 
-    def drag(self, direction='right', count=1):
-        '''滑动屏幕，适合一大块区域（如引导屏）的滑动，无需关心具体的控件
+    def drag(self, direction="right", count=1):
+        """滑动屏幕，适合一大块区域（如引导屏）的滑动，无需关心具体的控件
         
         :param direction: 方向，right、left、top、bottom
         :type  direction: string
         :param count:     次数
         :type  count:     int
-        '''
+        """
         width, height = self.device.screen_size
         mid_width = width // 2
         mid_height = height // 2
         x1 = x2 = mid_width
         y1 = y2 = mid_height
-        if direction == 'right':
+        if direction == "right":
             x1 -= 50
             x2 += 50
-        elif direction == 'left':
+        elif direction == "left":
             x1 += 50
             x2 -= 50
-        elif direction == 'top':
+        elif direction == "top":
             y1 += 50
             y2 -= 50
-        elif direction == 'bottom':
+        elif direction == "bottom":
             y1 -= 50
             y2 += 50
         else:
-            raise RuntimeError('不支持的方向：%s' % direction)
+            raise RuntimeError("不支持的方向：%s" % direction)
 
         for _ in range(count):
             self.get_driver().drag(x1, y1, x2, y2)
             time.sleep(0.5)
 
     def send_back_key(self):
-        '''发送返回按键
-        '''
+        """发送返回按键
+        """
         if self.device.is_rooted():
             self.device.send_key(4)
         else:
             res = self.device.send_key(4)
             if not res:
-                logger.info('send key 4 return False')
-                self.run_shell_cmd('input keyevent 4')
-            
+                logger.info("send key 4 return False")
+                self.run_shell_cmd("input keyevent 4")
+
     def send_key(self, key):
-        '''发送单个按键
+        """发送单个按键
         
         :param key: 发送的按键字符串
         :type  key: string
-        '''
+        """
         self.get_driver().send_key(key)
-        
+
     def send_home_key(self):
-        '''发送Home键
-        '''
+        """发送Home键
+        """
         self._device.send_key(3)
-        
+
     def send_menu_key(self):
-        '''发送菜单键
-        '''
-        self.get_driver().send_key('{MENU}')
-    
+        """发送菜单键
+        """
+        self.get_driver().send_key("{MENU}")
+
     def send_enter_key(self):
-        '''发送回车键
-        '''
-        self._device.send_text('\n')
-        
+        """发送回车键
+        """
+        self._device.send_text("\n")
+
     def close(self):
-        '''关闭所有打开的driver
-        '''
+        """关闭所有打开的driver
+        """
         self.remove_all_task()
         self.stop_monitor()
         for key in self._drivers.keys():
             self._drivers[key].close()
         self._drivers = {}
-    
+
     def run_shell_cmd(self, cmdline, **kwargs):
-        '''root下使用root权限执行命令，非root下使用应用权限执行命令
-        '''
+        """root下使用root权限执行命令，非root下使用应用权限执行命令
+        """
         if self._device.is_rooted():
             return self._device.run_shell_cmd(cmdline, True, **kwargs)
         else:
             return self._device.run_as(self.package_name, cmdline, **kwargs)
 
     def _close_other_window(self):
-        '''关闭会影响用例执行的窗口
-        '''
+        """关闭会影响用例执行的窗口
+        """
         current_activity = self.device.get_current_activity()
-        logger.debug('current_activity: %s' % current_activity)
+        logger.debug("current_activity: %s" % current_activity)
         if current_activity:
             pattern = re.compile(AppNoResponseWindow.Activity)
-            if current_activity == 'StatusBar':
+            if current_activity == "StatusBar":
                 self.send_back_key()
-            elif current_activity == CrashWindow.Activity or pattern.match(current_activity) or 'Application Not Responding' in current_activity:
+            elif (
+                current_activity == CrashWindow.Activity
+                or pattern.match(current_activity)
+                or "Application Not Responding" in current_activity
+            ):
                 # 如果是Crash窗口
                 self.device.send_key(66)
                 timeout = 10
                 time0 = time.time()
                 while time.time() - time0 < timeout:  # 等待窗口消失
                     current_activity = self.device.get_current_activity()
-                    if current_activity and (current_activity == CrashWindow.Activity or pattern.match(current_activity) or 'Application Not Responding' in current_activity):
+                    if current_activity and (
+                        current_activity == CrashWindow.Activity
+                        or pattern.match(current_activity)
+                        or "Application Not Responding" in current_activity
+                    ):
                         time.sleep(0.5)
                         self.device.send_key(66)
                     else:
                         return
                 self.device.send_key(4)
-            elif not '.' in current_activity:
+            elif not "." in current_activity:
                 # 一般这种情况是某种弹窗
                 timeout = 10
                 time0 = time.time()
-                while not '.' in current_activity and time.time() - time0 < timeout:  # 等待窗口消失
+                while (
+                    not "." in current_activity and time.time() - time0 < timeout
+                ):  # 等待窗口消失
                     self.device.send_key(61)
                     time.sleep(0.5)
                     self.device.send_key(66)
                     time.sleep(1)
                     current_activity = self.device.get_current_activity()
                     if not current_activity:  # 黑屏
                         time.sleep(3)
@@ -264,197 +293,241 @@
             while time.time() - time0 < timeout:
                 if not self.device.get_current_activity():
                     time.sleep(1)
                 else:
                     return
 
     def _detect_crash_window(self):
-        '''检测Crash窗口
-        '''
+        """检测Crash窗口
+        """
         current_activity = self.device.get_current_activity()
         if current_activity == CrashWindow.Activity:
             self.on_crashed()
             return True
 
     def on_crashed(self):
-        '''发生Crash之后的处理
-        '''
-        logger.error('detect crash')
+        """发生Crash之后的处理
+        """
+        logger.error("detect crash")
         self._app_crashed = True
         self._monitor_run = False
 
     def add_monitor_task(self, task, last_time=0, interval=1):
-        '''添加监控任务
-        '''
-        if last_time > 0: last_time += time.time()
-        task = {'task': task, 'end_time': last_time, 'interval': interval, 'last_exec_time': 0}
+        """添加监控任务
+        """
+        if last_time > 0:
+            last_time += time.time()
+        task = {
+            "task": task,
+            "end_time": last_time,
+            "interval": interval,
+            "last_exec_time": 0,
+        }
         self._monitor_task_list.append(task)
-        logger.debug('add task: %s' % task['task'].__name__)
-        
+        logger.debug("add task: %s" % task["task"].__name__)
+
     def remove_monitor_task(self, task):
-        '''移除监控任务
-        '''
+        """移除监控任务
+        """
         for item in self._monitor_task_list:
-            if item['task'] == task:
+            if item["task"] == task:
                 self._monitor_task_list.remove(item)
-                logger.debug('remove task: %s' % task.__name__)
+                logger.debug("remove task: %s" % task.__name__)
                 return True
         return False
 
     def remove_all_task(self):
-        '''移除所有任务
-        '''
+        """移除所有任务
+        """
         self._monitor_task_list = []
-    
+
     def start_monitor(self):
-        '''启动监控
-        '''
-        if self._monitor_thread: return
+        """启动监控
+        """
+        if self._monitor_thread:
+            return
         self._monitor_run = True
-        t = ThreadEx(target=self.monitor_thread, name='QT4A App Monitor Thread')
+        t = ThreadEx(target=self.monitor_thread, name="QT4A App Monitor Thread")
         t.setDaemon(True)
         t.start()
         self._monitor_thread = t
         self._device.adb.add_no_log_thread(t)
-        
+
     def stop_monitor(self):
-        '''停止检测
-        '''
-        if not hasattr(self, '_monitor_thread') or self._monitor_thread: return
+        """停止检测
+        """
+        if not hasattr(self, "_monitor_thread") or self._monitor_thread:
+            return
         self._monitor_run = False
         if self._monitor_thread.is_alive():
             self._monitor_thread.join(30)
         self._device.adb.remove_no_log_thread(self._monitor_thread)
         self._monitor_thread = None
-        
+
     def monitor_thread(self):
-        '''监控线程
-        '''
+        """监控线程
+        """
         interval = 1
         while self._monitor_run:
             for task in self._monitor_task_list:
                 time_now = time.time()
-                if task['end_time'] == 0 or (task['end_time'] > 0 and time_now < task['end_time']):
-                    if time.time() - task['last_exec_time'] >= task['interval']:
+                if task["end_time"] == 0 or (
+                    task["end_time"] > 0 and time_now < task["end_time"]
+                ):
+                    if time.time() - task["last_exec_time"] >= task["interval"]:
                         try:
-                            task['task']()
+                            task["task"]()
                         except:
-                            logger.exception('run task %s failed' % task['task'].__name__)
+                            logger.exception(
+                                "run task %s failed" % task["task"].__name__
+                            )
                             self._resume_main_thread()  # 防止出错后主线程阻塞一段时间
-                        task['last_exec_time'] = time.time()
+                        task["last_exec_time"] = time.time()
             time.sleep(interval)
-        
-    def get_string_resource(self, string_id, lang=''):
-        '''获取字符串资源
+
+    def get_string_resource(self, string_id, lang=""):
+        """获取字符串资源
         
         :param string_id: 字符串ID
         :type string_id:  string
         :param lang: 字符串语言，默认为当前系统语言
         :type lang:  string
-        '''
+        """
         return self.device.get_string_resource(self.package_name, string_id, lang)
-    
+
     def _suspend_main_thread(self, max_wait_time=30):
-        '''阻塞主线程
-        '''
-        if self._main_thread_id == threading.current_thread().ident: return  # 避免卡死
+        """阻塞主线程
+        """
+        if self._main_thread_id == threading.current_thread().ident:
+            return  # 避免卡死
         for key in self._drivers.keys():
             driver = self._drivers[key]
             driver.suspend_thread(self._main_thread_id, max_wait_time)
-    
+
     def _resume_main_thread(self):
-        '''解锁主线程
-        '''
-        if self._main_thread_id == threading.current_thread().ident: return
+        """解锁主线程
+        """
+        if self._main_thread_id == threading.current_thread().ident:
+            return
         for key in self._drivers.keys():
             driver = self._drivers[key]
             driver.resume_thread(self._main_thread_id)
-    
+
     def is_debug(self):
-        '''是否是debug包
-        '''
+        """是否是debug包
+        """
         return self.device.is_debug_package(self.package_name)
-    
+
     def _is_use_int_view_id(self):
-        '''是否使用整型控件ID
-        '''
-        if hasattr(self, '_use_int_view_id'): return self._use_int_view_id
+        """是否使用整型控件ID
+        """
+        if hasattr(self, "_use_int_view_id"):
+            return self._use_int_view_id
         if not self.is_debug():
-            logger.debug('release version')
-            _, file_list = self.device.list_dir('/data/local/tmp')
+            logger.debug("release version")
+            _, file_list = self.device.list_dir("/data/local/tmp")
             for file in file_list:
-                if file['name'] == '%s_map.txt' % self.package_name:
+                if file["name"] == "%s_map.txt" % self.package_name:
                     self._use_int_view_id = True
                     return True
-        logger.debug('map file not exist')
+        logger.debug("map file not exist")
         self._use_int_view_id = False
         return False
-    
+
     def _get_view_id(self, str_id):
-        '''从控件字符串ID获取整型ID
-        '''
-        if not str_id: raise RuntimeError('控件ID不能为空')
+        """从控件字符串ID获取整型ID
+        """
+        if not str_id:
+            raise RuntimeError("控件ID不能为空")
         try:
             return self.device._get_view_id(self.package_name, str_id)
         except RuntimeError as e:
             logger.warn(str(e))
             return None
-        
+
     def _get_drawable_resource_origin_name(self, confuse_name):
-        '''获取图片资源的原始名称
+        """获取图片资源的原始名称
         
         :param confuse_name: 混淆后的资源名称
         :type confuse_name:  string
-        '''
-        return self.device._get_resource_origin_name(self.package_name, 'drawable', confuse_name)
-    
-    def set_activity_popup(self, activity, popup=False, process_name=''):
-        '''设置Activity是否可以弹窗
-        '''
+        """
+        return self.device._get_resource_origin_name(
+            self.package_name, "drawable", confuse_name
+        )
+
+    def set_activity_popup(self, activity, popup=False, process_name=""):
+        """设置Activity是否可以弹窗
+        """
         return self.get_driver(process_name).set_activity_popup(activity, popup)
-    
+
     def send_image(self, activity, image_path):
-        '''向Activity发送图片，支持多图
+        """向Activity发送图片，支持多图
         
         :param activity:   目标Activity名称
         :type  activity:   string
         :param image_path: 图片在PC上的路径或路径列表
         :type  image_path: string | list
-        '''
-        self.device.send_image_to_app('%s/%s' % (self.package_name, activity), image_path)
-    
+        """
+        self.device.send_image_to_app(
+            "%s/%s" % (self.package_name, activity), image_path
+        )
+
     def send_file(self, activity, file_path):
-        '''向Activity发送文件
+        """向Activity发送文件
         
         :param activity:  目标Activity名称
         :type  activity:  string
         :param file_path: 文件在PC上的路径
         :type  file_path: string
-        '''
-        self.device.send_file_to_app('%s/%s' % (self.package_name, activity), file_path)
-    
-    def set_driver_thread_priority(self, process_name='', priority=EnumThreadPriority.FOREGROUND):
-        '''设置测试线程优先级
-        '''
+        """
+        self.device.send_file_to_app("%s/%s" % (self.package_name, activity), file_path)
+
+    def set_driver_thread_priority(
+        self, process_name="", priority=EnumThreadPriority.FOREGROUND
+    ):
+        """设置测试线程优先级
+        """
         self.get_driver(process_name).set_thread_priority(priority)
 
     def grant_all_runtime_permissions(self):
-        '''授予所有运行时权限
-        '''
-        if self.device.sdk_version < 23: return
+        """授予所有运行时权限
+        """
+        if self.device.sdk_version < 23:
+            return
         return self._device.grant_all_runtime_permissions(self.package_name)
-    
+
     def enable_system_alert_window(self):
-        '''允许弹出悬浮窗口
-        '''
-        return self._device.set_app_permission(self.package_name, 'SYSTEM_ALERT_WINDOW', True)
-    
+        """允许弹出悬浮窗口
+        """
+        return self._device.set_app_permission(
+            self.package_name, "SYSTEM_ALERT_WINDOW", True
+        )
+
     def enable_media_permission(self):
-        '''允许截屏和录音
+        """允许截屏和录音
         Capture the device's display contents and/or audio
-        '''
-        if self.device.sdk_version < 21: return
-        return self._device.set_app_permission(self.package_name, 'PROJECT_MEDIA', True)
+        """
+        if self.device.sdk_version < 21:
+            return
+        return self._device.set_app_permission(self.package_name, "PROJECT_MEDIA", True)
+
+    def dump_res_id_class_list(self):
+        app_root_path = "/data/data/%s" % self.package_name
+        r_id_file = "R_id.txt"
+        save_path = app_root_path + "/" + r_id_file
+        run_as = None
+        if not self._device.is_rooted():
+            run_as = self.package_name
+        _, file_list = self._device.adb.list_dir(app_root_path, run_as)
+
+        for it in file_list:
+            if it["name"] == r_id_file:
+                logger.info(
+                    "[%s] File %s exists" % (self.__class__.__name__, r_id_file)
+                )
+                return
+        self._device.dump_class_list(self.package_name, save_path, "R$id")
+
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     pass
```

### Comparing `qt4a-2.3.1/qt4a/androiddriver/__init__.py` & `qt4a-3.0.0/qt4a/androiddriver/__init__.py`

 * *Files identical despite different names*

### Comparing `qt4a-2.3.1/qt4a/androiddriver/_axmlparser.py` & `qt4a-3.0.0/qt4a/androiddriver/_axmlparser.py`

 * *Files identical despite different names*

### Comparing `qt4a-2.3.1/qt4a/androiddriver/adb.py` & `qt4a-3.0.0/qt4a/androiddriver/adb.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,59 +22,45 @@
 import re
 import six
 import subprocess
 import sys
 import threading
 import time
 
-from pkg_resources import iter_entry_points
 from qt4a.androiddriver.adbclient import ADBClient
 from qt4a.androiddriver.util import (
-    Singleton,
     Deprecated,
     logger,
     ThreadEx,
     TimeoutError,
     InstallPackageFailedError,
     PermissionError,
     is_int,
     utf8_encode,
     encode_wrap,
     enforce_utf8_decode,
     general_encode,
     time_clock,
+    get_command_path,
 )
 
 try:
     import _strptime  # time.strptime() is not thread-safed, so import _strptime first, otherwise it raises an AttributeError: _strptime_time
 except:
     pass
 cur_path = os.path.dirname(os.path.abspath(__file__))
 
 
 def get_adb_path():
-    if sys.platform == "win32":
-        sep = ";"
-        file_name = "adb.exe"
-    else:
-        sep = ":"
-        file_name = "adb"
-
-    path = os.environ.get("PATH")
-    if isinstance(path, bytes):
-        try:
-            path = path.decode("utf8")
-        except:
-            path = path.decode("gbk")
-    for root in path.split(sep):
-        adb_path = os.path.join(root, file_name)
-        if os.path.exists(adb_path):  # 优先使用环境变量中指定的 adb
-            return adb_path
-
-    return os.path.join(cur_path, "tools", "adb", sys.platform, file_name)
+    adb_path = get_command_path("adb")  # 优先使用环境变量中指定的 adb
+    if not adb_path:
+        adb_path = os.path.join(cur_path, "tools", "adb", sys.platform, "adb")
+        if sys.platform == "win32":
+            adb_path += ".exe"
+    return adb_path
 
 
 adb_path = get_adb_path()
 
 
 def is_adb_server_opend(host="localhost"):
     """判断ADB Server是否开启
@@ -82,15 +68,15 @@
     import socket
 
     sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
     try:
         sock.bind((host, 5037))
         sock.close()
         return False
-    except:
+    except Exception:
         return True
 
 
 class EnumRootState(object):
     """设备Root状态
     """
 
@@ -454,26 +440,27 @@
                 boot_complete = True
             else:
                 time.sleep(wait_period)
                 attempts += 1
         if not boot_complete:
             raise RuntimeError("dev.bootcomplete 标志在  %s 秒后仍未设置，手机重启失败" % _timeout)
 
-    def start_logcat(self, process_list=[], params=""):
+    def start_logcat(self, process_list=[], params="", clear=True):
         """运行logcat进程
         :param process_list: 要捕获日志的进程名或进程ID列表，为空则捕获所有进程
         :type process_list:  list
         """
         if not hasattr(self, "_start_count"):
             self._start_count = 0
         self._start_count += 1
         if self._start_count > 1:
             return
         logger.debug("[ADB] start logcat")
-        self.run_shell_cmd("logcat -c " + params)  # 清除缓冲区
+        if clear:
+            self.run_shell_cmd("logcat -c " + params)  # 清除缓冲区
         if not hasattr(self, "_log_list"):
             self._log_list = []
         self._logcat_running = True
         self._log_pipe = self.run_shell_cmd(
             "logcat -v threadtime " + params, sync=False
         )
 
@@ -545,15 +532,15 @@
         f = open(save_path, "wb")
         f.write(b"\n".join(log_list))
         f.close()
 
     def add_logcat_callback(self, callback):
         """添加logcat回调
         """
-        if not callback in self._logcat_callbacks:
+        if callback not in self._logcat_callbacks:
             self._logcat_callbacks.append(callback)
 
     def remove_logcat_callback(self, callback):
         """移除logcat回调
         """
         if callback in self._logcat_callbacks:
             self._logcat_callbacks.remove(callback)
@@ -651,15 +638,15 @@
 
             pid = int(ret.group(3))
             if pid in filter_pid_list:
                 continue
 
             init_process_list = ["<pre-initialized>", "zygote"]
 
-            if not pid in pid_dict.keys():
+            if pid not in pid_dict.keys():
                 for item in self.list_process():
                     if (
                         zygote_pid == 0
                         and item["proc_name"] == "zygote"
                         and item["ppid"] == 1
                     ):
                         # zygote父进程ID为1
@@ -675,15 +662,15 @@
                             for i in range(len(self._log_list) - 1, -1, -1):
                                 # 修复之前记录的“<pre-initialized>”进程
                                 pre_process_name = "[%s(%d)]" % (
                                     init_process,
                                     item["pid"],
                                 )
                                 pre_process_name = pre_process_name.encode("utf8")
-                                if not pre_process_name in self._log_list[i]:
+                                if pre_process_name not in self._log_list[i]:
                                     continue
                                 if process_list:
                                     del_flag = True
                                     for process in process_list:
                                         if pid == process or item[
                                             "proc_name"
                                         ].startswith(process):
@@ -711,15 +698,15 @@
                                     new_process_name = new_process_name.encode("utf8")
                                     self._log_list[i] = self._log_list[i].replace(
                                         pre_process_name, new_process_name
                                     )
                     pid_dict[item["pid"]] = item["proc_name"]
                 #                     if item['proc_name'] in init_process_list and item['pid'] != zygote_pid:
                 #                         pid_dict[item['pid']] += '(%d)' % item['pid']
-                if not pid in pid_dict.keys():
+                if pid not in pid_dict.keys():
                     filter_pid_list.append(pid)
                     continue
 
             found = False
             if not process_list:
                 found = True  # 不指定进程列表则捕获所有进程
             else:
@@ -1176,14 +1163,36 @@
                 param = "-" + param
             extra_str += param
         if len(extra_str) > 0:
             extra_str = extra_str[:-1]
         return extra_str
 
     @encode_wrap
+    def get_package_launcher_activity(self, package_name):
+        """获取一个应用的LAUNCHER activity
+        package_name: 包名
+        """
+        if not package_name:
+            raise RuntimeError("Invalid package name")
+
+        command = "dumpsys package {}".format(package_name)
+        result = self.run_shell_cmd(command, timeout=15, retry_count=3)
+
+        res = re.search(
+            r"android.intent.action.MAIN:.*?({}.*?) filter .*? "
+            r'Action: "android.intent.action.MAIN".*?Category: '
+            r'"android.intent.category.LAUNCHER"'.format(package_name),
+            result,
+            re.S,
+        )
+        if not res:
+            raise RuntimeError("package LAUNCHER activity not found")
+        return res.group(1)
+
+    @encode_wrap
     def start_activity(
         self, activity_name, action="", type="", data_uri="", extra={}, wait=True
     ):
         """打开一个Activity
         Warning: Activity not started, intent has been delivered to currently running top-most instance.
         Status: ok
         ThisTime: 0
@@ -1403,17 +1412,17 @@
             parent_path = "/".join(file_path.split("/")[:-1])
             dir_list, _ = self.list_dir(parent_path)
             for dir in dir_list:
                 if dir["name"] == dir_name:
                     new_attr = dir["attr"]
                     break
 
-        if new_attr != _parse(attr):
-            logger.warn("chmod failed: %r(%s)" % (ret, new_attr))
-            return self.chmod(file_path, attr)
+        # if new_attr != _parse(attr):
+        #     logger.warn("chmod failed: %r(%s)" % (ret, new_attr))
+        #     return self.chmod(file_path, attr)
         return new_attr
 
     def chown(self, file_path, uid, gid):
         """修改文件的拥有者和群组
 
         :param file_path: 文件路径
         :type file_path:  string
@@ -1436,29 +1445,36 @@
         except RuntimeError as e:
             logger.warn("mkdir %s failed: %s(%s)" % (dir_path, ret, e))
             return self.mkdir(dir_path, mod)
         # 修改权限
         if mod != None:
             self.chmod(dir_path, mod)
 
-    def list_dir(self, dir_path):
+    def list_dir(self, dir_path, run_as=None):
         """列取目录
         """
         if " " in dir_path:
             dir_path = '"%s"' % dir_path
-        use_root = self.is_rooted()
-        if (
-            use_root
-            and dir_path.startswith("/sdcard")
-            or dir_path.startswith("/storage/")
-            or dir_path.startswith("/mnt/")
-        ):
-            # 部分手机上发现用root权限访问/sdcard路径不一致
-            use_root = False
-        result = self.run_shell_cmd("ls -l %s" % dir_path, use_root)
+        cmdline = "ls -l %s" % dir_path
+
+        if run_as:
+            result = self.run_as(run_as, cmdline)
+        else:
+            use_root = self.is_rooted()
+
+            if (
+                use_root
+                and dir_path.startswith("/sdcard")
+                or dir_path.startswith("/storage/")
+                or dir_path.startswith("/mnt/")
+            ):
+                # 部分手机上发现用root权限访问/sdcard路径不一致
+                use_root = False
+
+            result = self.run_shell_cmd(cmdline, use_root)
 
         if "Permission denied" in result:
             raise PermissionError(result)
         if "No such file or directory" in result:
             raise RuntimeError("file or directory %s not exist" % dir_path)
         if "Not a directory" in result:
             raise RuntimeError("%s %s" % (dir_path, result))
```

### Comparing `qt4a-2.3.1/qt4a/androiddriver/adbclient.py` & `qt4a-3.0.0/qt4a/androiddriver/adbclient.py`

 * *Files identical despite different names*

### Comparing `qt4a-2.3.1/qt4a/androiddriver/androiddriver.py` & `qt4a-3.0.0/qt4a/androiddriver/androiddriver.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,36 +14,36 @@
 #
 
 """Android测试桩代理
 """
 from __future__ import print_function
 
 import base64
-import json
 import re
 import os
-import six
-import sys
 import tempfile
 import threading
 import time
 
+from qt4a.androiddriver.adb import ADB
 from qt4a.androiddriver.clientsocket import DirectAndroidSpyClient
 from qt4a.androiddriver.devicedriver import DeviceDriver
 from qt4a.androiddriver.util import (
-    logger,
-    general_encode,
-    SocketError,
+    AndroidPackage,
     AndroidSpyError,
     ControlAmbiguousError,
     ControlExpiredError,
     ProcessExitError,
     QT4ADriverNotInstalled,
+    SocketError,
     Mutex,
+    logger,
+    general_encode,
     extract_from_zipfile,
+    version_cmp,
 )
 
 
 class EnumCommand(object):
     """所有支持的命令字
     """
 
@@ -81,16 +81,14 @@
     CmdCallExternalMethod = "CallExternalMethod"  # 调用外部jar包中的方法
     CmdSetActivityPopup = "SetActivityPopup"
     CmdSetThreadPriority = "SetThreadPriority"
     CmdSetWebViewDebuggingEnabled = "SetWebViewDebuggingEnabled"
 
 
 def install_qt4a_helper(adb, root_path):
-    from qt4a.androiddriver.util import AndroidPackage, version_cmp
-
     qt4a_helper_package = "com.test.androidspy"
     apk_path = os.path.join(root_path, "QT4AHelper.apk")
     if adb.get_package_path(qt4a_helper_package):
         # 判断版本
         installed_version = adb.get_package_version(qt4a_helper_package)
         package = AndroidPackage(apk_path)
         install_version = package.version
@@ -99,16 +97,14 @@
     else:
         adb.install_apk(apk_path)
 
 
 def copy_android_driver(device_id_or_adb, force=False, root_path=None, enable_acc=True):
     """测试前的测试桩拷贝
     """
-    from qt4a.androiddriver.adb import ADB
-
     if isinstance(device_id_or_adb, ADB):
         adb = device_id_or_adb
     else:
         adb = ADB.open_device(device_id_or_adb)
 
     if not root_path:
         current_path = os.path.abspath(__file__)
@@ -133,25 +129,25 @@
 
     if not force:
         version_file = dst_path + "version.txt"
         version = adb.run_shell_cmd("cat %s" % version_file)
 
         if (
             version
-            and not "No such file or directory" in version
+            and "No such file or directory" not in version
             and current_version <= int(version)
         ):
             install_qt4a_helper(adb, root_path)  # 避免QT4A助手被意外删除的情况
             # 不需要拷贝测试桩
             logger.warn("忽略本次测试桩拷贝：当前版本为%s，设备中版本为%s" % (current_version, int(version)))
             return
 
     try:
         adb.chmod(dst_path[:-1], "777")
-    except:
+    except Exception:
         pass
 
     rooted = adb.is_rooted()
 
     cpu_abi = adb.get_cpu_abi()
     print("Current CPU arch: %s" % cpu_abi)
     # use_pie = False
@@ -163,44 +159,46 @@
         os.path.join(cpu_abi, "libdexloader.so"),
         os.path.join(cpu_abi, "screenkit"),
         "inject",
         "AndroidSpy.jar",
         "SpyHelper.jar",
         "SpyHelper.sh",
     ]
-    if cpu_abi == "arm64-v8a":
+
+    if adb.get_sdk_version() >= 21:
+        file_list.append(os.path.join(cpu_abi, "libandroidhook.so"))
+
+    if cpu_abi in ("x86_64", "arm64-v8a"):
         file_list.append(os.path.join(cpu_abi, "droid_inject64"))
         file_list.append(os.path.join(cpu_abi, "libdexloader64.so"))
         file_list.append("inject64")
-    if adb.get_sdk_version() >= 21:
-        file_list.append(os.path.join(cpu_abi, "libandroidhook_art.so"))
+        if adb.get_sdk_version() >= 21:
+            file_list.append(os.path.join(cpu_abi, "libandroidhook64.so"))
 
     if rooted and adb.is_selinux_opened():
         # 此时如果还是开启状态说明关闭selinux没有生效,主要是三星手机上面
         adb.run_shell_cmd("rm -r %s" % dst_path, True)
         # adb.run_shell_cmd('chcon u:object_r:shell_data_file:s0 %slibdexloader.so' % dst_path, True)  # 恢复文件context，否则拷贝失败
         # adb.run_shell_cmd('chcon u:object_r:shell_data_file:s0 %slibandroidhook.so' % dst_path, True)
 
     for file in file_list:
         file_path = os.path.join(root_path, file)
         # if use_pie and not "." in file and os.path.exists(file_path + "_pie"):
         #     file_path += "_pie"
         if not os.path.exists(file_path):
             continue
         save_name = os.path.split(file)[-1]
-        if save_name.endswith("_art.so"):
-            save_name = save_name.replace("_art", "")
         adb.push_file(file_path, dst_path + save_name)
 
     adb.chmod("%sdroid_inject" % dst_path, 755)
     adb.chmod("%sinject" % dst_path, 755)
     adb.chmod("%sscreenkit" % dst_path, 755)
     adb.run_shell_cmd("ln -s %sscreenkit %sscreenshot" % (dst_path, dst_path))
 
-    if cpu_abi == "arm64-v8a":
+    if cpu_abi in ("arm64-v8a", "x86_64"):
         adb.chmod("%sdroid_inject64" % dst_path, 755)
         adb.chmod("%sinject64" % dst_path, 755)
 
     try:
         print(adb.run_shell_cmd("rm -R %scache" % dst_path, rooted))  # 删除目录 rm -rf
     except RuntimeError as e:
         logger.warn("%s" % e)
@@ -265,15 +263,15 @@
                     "sh %sSpyHelper.sh loadDex %sAndroidSpy.jar %scache"
                     % (dst_path, dst_path, dst_path),
                     rooted,
                 )
             )
             adb.chmod("%scache/AndroidSpy.dex" % dst_path, 666)
     else:
-        if not "usage:" in adb.run_shell_cmd("sh %sSpyHelper.sh" % dst_path):
+        if "usage:" not in adb.run_shell_cmd("sh %sSpyHelper.sh" % dst_path):
             adb.mkdir("%scache/dalvik-cache" % dst_path, 777)
 
     if rooted and adb.is_selinux_opened() and adb.get_sdk_version() >= 23:
         # 提升权限
         try:
             adb.list_dir("/system/bin/app_process32")
         except RuntimeError:
@@ -302,20 +300,20 @@
         if enable_acc:
             device_driver.modify_system_setting(
                 "secure",
                 "enabled_accessibility_services",
                 "com.test.androidspy/com.test.androidspy.service.QT4AAccessibilityService",
             )
             device_driver.modify_system_setting("secure", "accessibility_enabled", 1)
-    except:
+    except Exception:
         logger.exception("set default input method failed")
     try:
         device_driver.modify_system_setting("system", "time_12_24", 24)
         device_driver.modify_system_setting("system", "screen_off_timeout", 600 * 1000)
-    except:
+    except Exception:
         logger.exception("set system time failed")
 
 
 class AndroidDriver(object):
     """
     """
 
@@ -579,15 +577,14 @@
         """发送命令
         """
         curr_thread_id = threading.current_thread().ident
         self._wait_for_event(curr_thread_id, self._max_block_time)
 
         if cmd_type != EnumCommand.CmdHello:
             self._safe_init_driver()  # 确保测试桩连接正常
-
         result = self._client.send_command(cmd_type, **kwds)
         if result == None:
             pid = self._adb.get_pid(self._process["name"])
             if pid > 0 and pid != self._process["id"]:
                 # 新进程，需要重新注入
                 logger.info(
                     "process %s id changed: %d %d"
@@ -629,15 +626,14 @@
             except SocketError:
                 time.sleep(1)
                 continue
             except AndroidSpyError:
                 logger.exception("init error")
                 time.sleep(2)
                 continue
-            # self._enable_debug()
             if not "Result" in result:
                 raise RuntimeError("Server error")
             items = result["Result"].split(":")
             if len(items) > 0 and items[-1].isdigit():
                 if self._process["id"] and int(items[-1]) != self._process["id"]:
                     raise RuntimeError("Server pid not match %s" % result["Result"])
             return result["Result"]
```

### Comparing `qt4a-2.3.1/qt4a/androiddriver/clientsocket.py` & `qt4a-3.0.0/qt4a/androiddriver/clientsocket.py`

 * *Files identical despite different names*

### Comparing `qt4a-2.3.1/qt4a/androiddriver/devicedriver.py` & `qt4a-3.0.0/qt4a/androiddriver/devicedriver.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     def run_driver_cmd(self, cmd, *args, **kwargs):
         """执行驱动命令
         
         :param cmd:  命令
         :type  cmd:  string
         """
         args = [
-            ('"%s"' % (it.replace('"', r"\"") if isinstance(it, str) else it))
+            ("'%s'" % (it.replace("'", r"\'") if isinstance(it, str) else it))
             for it in args
         ]
         result = self.adb.run_shell_cmd(
             "sh %s/SpyHelper.sh %s %s" % (qt4a_path, cmd, " ".join(args)), **kwargs
         )
         if "No such file or directory" in result:
             raise QT4ADriverNotInstalled("Please install QT4A driver first")
@@ -127,16 +127,20 @@
         :param pkg_size:  安装包大小
         :type pkg_size:   int
         :param pkg_md5:   安装包md5
         :type pkg_md5:    string
         """
         timeout = 60
         ret = self.run_driver_cmd(
-            "isPackageInstalled", pkg_name, pkg_size, pkg_md5, root=self.adb.is_rooted(),
-            timeout=timeout
+            "isPackageInstalled",
+            pkg_name,
+            pkg_size,
+            pkg_md5,
+            root=self.adb.is_rooted(),
+            timeout=timeout,
         )
         return "true" in ret
 
     def install_package(self, pkg_path, overwrite=False):
         """安装应用
         """
         from qt4a.androiddriver.util import get_file_md5
@@ -231,27 +235,27 @@
         if self.adb.get_sdk_version() >= 29:
             result = self.adb.run_shell_cmd("dumpsys window visible-apps")
         else:
             result = self.adb.run_shell_cmd("dumpsys window")
         if result:
             line_list = result.split("\n")
             for line in line_list:
-                if "mCurrentFocus" in line or "mFocusedWindow" in line:
+                if "mCurrentFocus=Window" in line or "mFocusedWindow=Window" in line:
                     result = line
                     break
         pattern1 = re.compile(r"mCurrentFocus=Window{(.+)}")
         pattern2 = re.compile(r"mFocusedWindow=Window{(.+)}")
         for pattern in (pattern1, pattern2):
             ret = pattern.search(result)
             if ret:
                 break
         else:
             logger.info("Get current window by dumpsys failed: %s" % result)
             return None
-        result = ret.group(1).split(" ")[-1]
+        result = ret.group(1).split(" ")[2]
         if "/" in result:
             result = result.split("/")[-1]
         if "Application Not Responding" in ret.group(1):
             result = "Application Not Responding: %s" % result
         return result
 
     def get_current_activity(self):
@@ -295,26 +299,31 @@
                 return result["Width"], result["Height"]
 
         result = self.run_driver_cmd("getScreenSize", root=self.adb.is_rooted())
         result = result.split("\n")[-1]
         width, height = result.split(",")
         return int(width), int(height)
 
-    def _take_screen_shot(self, path, _format='png', quality=90):
+    def _take_screen_shot(self, path, _format="png", quality=90):
         """
         使用android系统命令截图
         # todo:使用android的java接口替换该方案
         """
         # result = self.adb.run_shell_cmd(
         #     "sh %s/SpyHelper.sh takeScreenshot %s %s %s" % (qt4a_path, path, _format, quality), self.adb.is_rooted())
         # if 'true' in result:
         #     return True
         # logger.warn("Take screenshot by SpyHelper.sh failed: %s" % result)
         try:
-            result = self.adb.run_shell_cmd("screencap -p", binary_output=True)
+            img_path = qt4a_path + "/screen.png"
+            # result = self.adb.run_shell_cmd("screencap -p", binary_output=True)
+            screen_img = self.adb.run_shell_cmd("screencap -p %s" % (img_path))
+            pull_img = self.adb.pull_file(img_path, path)
+            with open(path, "rb") as fp:
+                result = fp.read()
             return result
         except Exception as e:
             logger.warn("Take screenshot failed: %s" % traceback.format_exc(e))
             return False
 
     def take_screen_shot(self, path, quality=90):
         """截屏
@@ -1192,10 +1201,35 @@
         :type  zip_file: string
         :param save_dir: 保存目录路径
         :type  save_dir: string
         """
         result = self.run_driver_cmd("unzip", zip_file, save_dir)
         return "true" in result
 
+    def dump_class_list(self, package_name, save_path, filter=None):
+        """Dump应用中的类列表
+
+        :param package_name: 应用包名
+        :type  package_name: string
+        :param save_path: 保存路径
+        :type  save_path: string
+        :param filter: 类名过滤器
+        "type  filter: string
+        """
+        tmp_save_path = "/data/local/tmp/R_id.txt"
+        result = self.run_driver_cmd(
+            "dumpClassList", package_name, tmp_save_path, filter or ""
+        )
+        logger.debug(
+            "[%s] Dump class of %s result: \n%s"
+            % (self.__class__.__name__, package_name, result)
+        )
+        self.adb.chmod(tmp_save_path, 755)
+        cmdline = "cp %s '%s'" % (tmp_save_path, save_path)
+        if self.adb.is_rooted():
+            self.adb.run_shell_cmd(cmdline, root=True)
+        else:
+            self.adb.run_as(package_name, cmdline)
+
 
 if __name__ == "__main__":
     pass
```

### Comparing `qt4a-2.3.1/qt4a/androiddriver/tools/SpyHelper.sh` & `qt4a-3.0.0/qt4a/androiddriver/tools/SpyHelper.sh`

 * *Files identical despite different names*

### Comparing `qt4a-2.3.1/qt4a/androiddriver/tools/adb/darwin/adb` & `qt4a-3.0.0/qt4a/androiddriver/tools/adb/darwin/adb`

 * *Files identical despite different names*

### Comparing `qt4a-2.3.1/qt4a/androiddriver/tools/adb/linux2/adb` & `qt4a-3.0.0/qt4a/androiddriver/tools/adb/linux2/adb`

 * *Files identical despite different names*

### Comparing `qt4a-2.3.1/qt4a/androiddriver/tools/adb/win32/AdbWinApi.dll` & `qt4a-3.0.0/qt4a/androiddriver/tools/adb/win32/AdbWinApi.dll`

 * *Files identical despite different names*

### Comparing `qt4a-2.3.1/qt4a/androiddriver/tools/adb/win32/AdbWinUsbApi.dll` & `qt4a-3.0.0/qt4a/androiddriver/tools/adb/win32/AdbWinUsbApi.dll`

 * *Files identical despite different names*

### Comparing `qt4a-2.3.1/qt4a/androiddriver/tools/adb/win32/adb.exe` & `qt4a-3.0.0/qt4a/androiddriver/tools/adb/win32/adb.exe`

 * *Files identical despite different names*

### Comparing `qt4a-2.3.1/qt4a/androiddriver/tools/androidhook.jar` & `qt4a-3.0.0/qt4a/androiddriver/tools/androidhook.jar`

 * *Files identical despite different names*

### Comparing `qt4a-2.3.1/qt4a/androiddriver/tools/arm64-v8a/droid_inject` & `qt4a-3.0.0/qt4a/androiddriver/tools/arm64-v8a/droid_inject`

 * *Files identical despite different names*

### Comparing `qt4a-2.3.1/qt4a/androiddriver/tools/arm64-v8a/droid_inject64` & `qt4a-3.0.0/qt4a/androiddriver/tools/arm64-v8a/droid_inject64`

 * *Files identical despite different names*

### Comparing `qt4a-2.3.1/qt4a/androiddriver/tools/arm64-v8a/libdexloader64.so` & `qt4a-3.0.0/qt4a/androiddriver/tools/arm64-v8a/libdexloader64.so`

 * *Files 26% similar despite different names*

#### readelf --wide --file-header {}

```diff
@@ -4,17 +4,17 @@
   Data:                              2's complement, little endian
   Version:                           1 (current)
   OS/ABI:                            UNIX - System V
   ABI Version:                       0
   Type:                              DYN (Shared object file)
   Machine:                           AArch64
   Version:                           0x1
-  Entry point address:               0xfd0
+  Entry point address:               0x1320
   Start of program headers:          64 (bytes into file)
-  Start of section headers:          12488 (bytes into file)
+  Start of section headers:          12608 (bytes into file)
   Flags:                             0x0
   Size of this header:               64 (bytes)
   Size of program headers:           56 (bytes)
-  Number of program headers:         6
+  Number of program headers:         8
   Size of section headers:           64 (bytes)
-  Number of section headers:         19
-  Section header string table index: 18
+  Number of section headers:         22
+  Section header string table index: 21
```

#### readelf --wide --program-header {}

```diff
@@ -1,22 +1,26 @@
 
 Elf file type is DYN (Shared object file)
-Entry point 0xfd0
-There are 6 program headers, starting at offset 64
+Entry point 0x1320
+There are 8 program headers, starting at offset 64
 
 Program Headers:
   Type           Offset   VirtAddr           PhysAddr           FileSiz  MemSiz   Flg Align
-  LOAD           0x000000 0x0000000000000000 0x0000000000000000 0x0023b0 0x0023b0 R E 0x10000
-  LOAD           0x002cc0 0x0000000000012cc0 0x0000000000012cc0 0x000348 0x000348 RW  0x10000
-  DYNAMIC        0x002cd8 0x0000000000012cd8 0x0000000000012cd8 0x0001f0 0x0001f0 RW  0x8
-  GNU_EH_FRAME   0x002158 0x0000000000002158 0x0000000000002158 0x000054 0x000054 R   0x4
+  LOAD           0x000000 0x0000000000000000 0x0000000000000000 0x002ae0 0x002ae0 R E 0x10000
+  LOAD           0x002c60 0x0000000000012c60 0x0000000000012c60 0x0003a8 0x0003a8 RW  0x10000
+  DYNAMIC        0x002c78 0x0000000000012c78 0x0000000000012c78 0x000210 0x000210 RW  0x8
+  NOTE           0x000200 0x0000000000000200 0x0000000000000200 0x000024 0x000024 R   0x4
+  NOTE           0x002a48 0x0000000000002a48 0x0000000000002a48 0x000098 0x000098 R   0x4
+  GNU_EH_FRAME   0x002810 0x0000000000002810 0x0000000000002810 0x00006c 0x00006c R   0x4
   GNU_STACK      0x000000 0x0000000000000000 0x0000000000000000 0x000000 0x000000 RW  0x10
-  GNU_RELRO      0x002cc0 0x0000000000012cc0 0x0000000000012cc0 0x000340 0x000340 R   0x1
+  GNU_RELRO      0x002c60 0x0000000000012c60 0x0000000000012c60 0x0003a0 0x0003a0 R   0x1
 
  Section to Segment mapping:
   Segment Sections...
-   00     .hash .dynsym .dynstr .rela.dyn .rela.plt .plt .text .rodata .eh_frame_hdr .eh_frame 
+   00     .note.gnu.build-id .hash .dynsym .dynstr .gnu.version .gnu.version_r .rela.dyn .rela.plt .plt .text .rodata .eh_frame_hdr .eh_frame .note.android.ident 
    01     .init_array .fini_array .dynamic .got .data 
    02     .dynamic 
-   03     .eh_frame_hdr 
-   04     
-   05     .init_array .fini_array .dynamic .got 
+   03     .note.gnu.build-id 
+   04     .note.android.ident 
+   05     .eh_frame_hdr 
+   06     
+   07     .init_array .fini_array .dynamic .got
```

#### readelf --wide --sections {}

```diff
@@ -1,28 +1,31 @@
-There are 19 section headers, starting at offset 0x30c8:
+There are 22 section headers, starting at offset 0x3140:
 
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
-  [ 1] .hash             HASH            0000000000000190 000190 000170 04   A  2   0  8
-  [ 2] .dynsym           DYNSYM          0000000000000300 000300 0004f8 18   A  3   3  8
-  [ 3] .dynstr           STRTAB          00000000000007f8 0007f8 00023c 00   A  0   0  1
-  [ 4] .rela.dyn         RELA            0000000000000a38 000a38 000048 18   A  2   0  8
-  [ 5] .rela.plt         RELA            0000000000000a80 000a80 000318 18  AI  2   6  8
-  [ 6] .plt              PROGBITS        0000000000000da0 000da0 000230 10  AX  0   0 16
-  [ 7] .text             PROGBITS        0000000000000fd0 000fd0 000d7c 00  AX  0   0  4
-  [ 8] .rodata           PROGBITS        0000000000001d50 001d50 000408 01 AMS  0   0  8
-  [ 9] .eh_frame_hdr     PROGBITS        0000000000002158 002158 000054 00   A  0   0  4
-  [10] .eh_frame         PROGBITS        00000000000021b0 0021b0 000200 00   A  0   0  8
-  [11] .init_array       INIT_ARRAY      0000000000012cc0 002cc0 000008 00  WA  0   0  1
-  [12] .fini_array       FINI_ARRAY      0000000000012cc8 002cc8 000010 00  WA  0   0  8
-  [13] .dynamic          DYNAMIC         0000000000012cd8 002cd8 0001f0 10  WA  3   0  8
-  [14] .got              PROGBITS        0000000000012ec8 002ec8 000138 08  WA  0   0  8
-  [15] .data             PROGBITS        0000000000013000 003000 000008 00  WA  0   0  8
-  [16] .bss              NOBITS          0000000000013008 003008 000000 00  WA  0   0  1
-  [17] .comment          PROGBITS        0000000000000000 003008 000025 01  MS  0   0  1
-  [18] .shstrtab         STRTAB          0000000000000000 00302d 000095 00      0   0  1
+  [ 1] .note.gnu.build-id NOTE            0000000000000200 000200 000024 00   A  0   0  4
+  [ 2] .hash             HASH            0000000000000228 000228 000180 04   A  3   0  8
+  [ 3] .dynsym           DYNSYM          00000000000003a8 0003a8 000558 18   A  4   3  8
+  [ 4] .dynstr           STRTAB          0000000000000900 000900 00027f 00   A  0   0  1
+  [ 5] .gnu.version      VERSYM          0000000000000b80 000b80 000072 02   A  3   0  2
+  [ 6] .gnu.version_r    VERNEED         0000000000000bf8 000bf8 000040 00   A  4   2  8
+  [ 7] .rela.dyn         RELA            0000000000000c38 000c38 000030 18   A  3   0  8
+  [ 8] .rela.plt         RELA            0000000000000c68 000c68 0003f0 18  AI  3  18  8
+  [ 9] .plt              PROGBITS        0000000000001060 001060 0002c0 10  AX  0   0 16
+  [10] .text             PROGBITS        0000000000001320 001320 001028 00  AX  0   0  4
+  [11] .rodata           PROGBITS        0000000000002348 002348 0004c5 00   A  0   0  1
+  [12] .eh_frame_hdr     PROGBITS        0000000000002810 002810 00006c 00   A  0   0  4
+  [13] .eh_frame         PROGBITS        0000000000002880 002880 0001c8 00   A  0   0  8
+  [14] .note.android.ident NOTE            0000000000002a48 002a48 000098 00   A  0   0  4
+  [15] .init_array       INIT_ARRAY      0000000000012c60 002c60 000008 08  WA  0   0  1
+  [16] .fini_array       FINI_ARRAY      0000000000012c68 002c68 000010 08  WA  0   0  8
+  [17] .dynamic          DYNAMIC         0000000000012c78 002c78 000210 10  WA  4   0  8
+  [18] .got              PROGBITS        0000000000012e88 002e88 000178 08  WA  0   0  8
+  [19] .data             PROGBITS        0000000000013000 003000 000008 00  WA  0   0  8
+  [20] .comment          PROGBITS        0000000000000000 003008 000064 01  MS  0   0  1
+  [21] .shstrtab         STRTAB          0000000000000000 00306c 0000d3 00      0   0  1
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
   D (mbind), p (processor specific)
```

#### readelf --wide --symbols {}

```diff
@@ -1,56 +1,60 @@
 
-Symbol table '.dynsym' contains 53 entries:
+Symbol table '.dynsym' contains 57 entries:
    Num:    Value          Size Type    Bind   Vis      Ndx Name
      0: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT  UND 
-     1: 0000000000000fd0     0 SECTION LOCAL  DEFAULT    7 .text
-     2: 0000000000013000     0 SECTION LOCAL  DEFAULT   15 .data
-     3: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND pthread_create
-     4: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND munmap
-     5: 0000000000000000     0 OBJECT  GLOBAL DEFAULT  UND __stack_chk_guard
-     6: 0000000000013008     0 NOTYPE  GLOBAL DEFAULT   16 _bss_end__
-     7: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND fgets
-     8: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND getc
-     9: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cxa_finalize
-    10: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND getuid
-    11: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND malloc
-    12: 0000000000013008     0 NOTYPE  GLOBAL DEFAULT   16 __bss_start__
-    13: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND strtoul
-    14: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __android_log_print
-    15: 0000000000001364   828 FUNC    GLOBAL DEFAULT    7 load_dex
-    16: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND mmap
-    17: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __stack_chk_fail
-    18: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND chmod
-    19: 0000000000001800   228 FUNC    GLOBAL DEFAULT    7 get_module_base
-    20: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND fstat
-    21: 0000000000013008     0 NOTYPE  GLOBAL DEFAULT   16 __bss_end__
-    22: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND umask
-    23: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND strstr
-    24: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND read
-    25: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND strncpy
-    26: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cxa_atexit
-    27: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND strtok
-    28: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND dlsym
-    29: 000000000000100c   856 FUNC    GLOBAL DEFAULT    7 load_dex_in_thread
-    30: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND fopen
-    31: 0000000000013008     0 NOTYPE  GLOBAL DEFAULT   16 __bss_start
-    32: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND memset
-    33: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND fclose
-    34: 0000000000001c18   308 FUNC    GLOBAL DEFAULT    7 get_jni_env
-    35: 0000000000013008     0 NOTYPE  GLOBAL DEFAULT   16 __end__
-    36: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND strcmp
-    37: 00000000000016c4    76 FUNC    GLOBAL DEFAULT    7 get_file_size
-    38: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND sprintf
-    39: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND fputc
-    40: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND stat
-    41: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND access
-    42: 0000000000013008     0 NOTYPE  GLOBAL DEFAULT   15 _edata
-    43: 0000000000013008     0 NOTYPE  GLOBAL DEFAULT   16 _end
-    44: 00000000000018e4   820 FUNC    GLOBAL DEFAULT    7 get_symbol_offset
-    45: 00000000000016a0     4 FUNC    GLOBAL DEFAULT    7 Java_com_test_androidspy_HelperUtil_nativeSetsid
-    46: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND open
-    47: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND setsid
-    48: 00000000000016a4    32 FUNC    GLOBAL DEFAULT    7 Java_com_test_androidspy_HelperUtil_nativeUmask
-    49: 0000000000001710   240 FUNC    GLOBAL DEFAULT    7 copyfile
-    50: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND mkdir
-    51: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND close
-    52: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND free
+     1: 0000000000001320     0 SECTION LOCAL  DEFAULT   10 .text
+     2: 0000000000013000     0 SECTION LOCAL  DEFAULT   19 .data
+     3: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND atoi@LIBC (2)
+     4: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND pthread_create@LIBC (2)
+     5: 0000000000013008     0 NOTYPE  GLOBAL DEFAULT  ABS _bss_end__
+     6: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND open@LIBC (2)
+     7: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND umask@LIBC (2)
+     8: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cxa_finalize@LIBC (2)
+     9: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND mkdir@LIBC (2)
+    10: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND read@LIBC (2)
+    11: 0000000000002174   468 FUNC    GLOBAL DEFAULT   10 setApiBlacklistExemptions
+    12: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND strtoul@LIBC (2)
+    13: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND fstat@LIBC (2)
+    14: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND chmod@LIBC (2)
+    15: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND setsid@LIBC (2)
+    16: 0000000000001b28    84 FUNC    GLOBAL DEFAULT   10 get_file_size
+    17: 00000000000019e8   216 FUNC    GLOBAL DEFAULT   10 JNI_OnLoad
+    18: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND access@LIBC (2)
+    19: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND fclose@LIBC (2)
+    20: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND fputc@LIBC (2)
+    21: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __stack_chk_fail@LIBC (2)
+    22: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND fgets@LIBC (2)
+    23: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND getc@LIBC (2)
+    24: 0000000000001b7c   228 FUNC    GLOBAL DEFAULT   10 copyfile
+    25: 0000000000001c60   204 FUNC    GLOBAL DEFAULT   10 get_module_base
+    26: 0000000000013008     0 NOTYPE  GLOBAL DEFAULT  ABS __bss_start
+    27: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND strncpy@LIBC (2)
+    28: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND dlsym@LIBC (3)
+    29: 0000000000013008     0 NOTYPE  GLOBAL DEFAULT  ABS __end__
+    30: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __android_log_print
+    31: 00000000000019cc    28 FUNC    GLOBAL DEFAULT   10 Java_com_test_androidspy_HelperUtil_nativeUmask
+    32: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND strcmp@LIBC (2)
+    33: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND sprintf@LIBC (2)
+    34: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND mmap@LIBC (2)
+    35: 0000000000001d2c   792 FUNC    GLOBAL DEFAULT   10 get_symbol_offset
+    36: 0000000000013008     0 NOTYPE  GLOBAL DEFAULT  ABS __bss_start__
+    37: 0000000000001ac0   104 FUNC    GLOBAL DEFAULT   10 get_sdk_version
+    38: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND getuid@LIBC (2)
+    39: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND strstr@LIBC (2)
+    40: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND strtok@LIBC (2)
+    41: 000000000000135c   896 FUNC    GLOBAL DEFAULT   10 load_dex_in_thread
+    42: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND close@LIBC (2)
+    43: 00000000000019c8     4 FUNC    GLOBAL DEFAULT   10 Java_com_test_androidspy_HelperUtil_nativeSetsid
+    44: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND stat@LIBC (2)
+    45: 00000000000016dc   748 FUNC    GLOBAL DEFAULT   10 load_dex
+    46: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND munmap@LIBC (2)
+    47: 0000000000013008     0 NOTYPE  GLOBAL DEFAULT  ABS _edata
+    48: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND malloc@LIBC (2)
+    49: 0000000000013008     0 NOTYPE  GLOBAL DEFAULT  ABS __bss_end__
+    50: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND memset@LIBC (2)
+    51: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND fopen@LIBC (2)
+    52: 0000000000013008     0 NOTYPE  GLOBAL DEFAULT  ABS _end
+    53: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND free@LIBC (2)
+    54: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __system_property_get@LIBC (2)
+    55: 0000000000002044   304 FUNC    GLOBAL DEFAULT   10 get_jni_env
+    56: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cxa_atexit@LIBC (2)
```

#### readelf --wide --relocs {}

```diff
@@ -1,42 +1,50 @@
 
-Relocation section '.rela.dyn' at offset 0xa38 contains 3 entries:
+Relocation section '.rela.dyn' at offset 0xc38 contains 2 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
-0000000000012cc8  0000000000000403 R_AARCH64_RELATIVE                        fd0
-0000000000012ff8  0000000000000403 R_AARCH64_RELATIVE                        100c
-0000000000012ff0  0000000500000401 R_AARCH64_GLOB_DAT     0000000000000000 __stack_chk_guard + 0
+0000000000012c68  0000000000000403 R_AARCH64_RELATIVE                        1320
+0000000000012ff8  0000002900000401 R_AARCH64_GLOB_DAT     000000000000135c load_dex_in_thread + 0
 
-Relocation section '.rela.plt' at offset 0xa80 contains 33 entries:
+Relocation section '.rela.plt' at offset 0xc68 contains 42 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
-0000000000012ee0  0000000300000402 R_AARCH64_JUMP_SLOT    0000000000000000 pthread_create + 0
-0000000000012ee8  0000000400000402 R_AARCH64_JUMP_SLOT    0000000000000000 munmap + 0
-0000000000012ef0  0000000700000402 R_AARCH64_JUMP_SLOT    0000000000000000 fgets + 0
-0000000000012ef8  0000000800000402 R_AARCH64_JUMP_SLOT    0000000000000000 getc + 0
-0000000000012f00  0000000900000402 R_AARCH64_JUMP_SLOT    0000000000000000 __cxa_finalize + 0
-0000000000012f08  0000000a00000402 R_AARCH64_JUMP_SLOT    0000000000000000 getuid + 0
-0000000000012f10  0000000b00000402 R_AARCH64_JUMP_SLOT    0000000000000000 malloc + 0
-0000000000012f18  0000000d00000402 R_AARCH64_JUMP_SLOT    0000000000000000 strtoul + 0
-0000000000012f20  0000000e00000402 R_AARCH64_JUMP_SLOT    0000000000000000 __android_log_print + 0
-0000000000012f28  0000001000000402 R_AARCH64_JUMP_SLOT    0000000000000000 mmap + 0
-0000000000012f30  0000001100000402 R_AARCH64_JUMP_SLOT    0000000000000000 __stack_chk_fail + 0
-0000000000012f38  0000001200000402 R_AARCH64_JUMP_SLOT    0000000000000000 chmod + 0
-0000000000012f40  0000001400000402 R_AARCH64_JUMP_SLOT    0000000000000000 fstat + 0
-0000000000012f48  0000001600000402 R_AARCH64_JUMP_SLOT    0000000000000000 umask + 0
-0000000000012f50  0000001700000402 R_AARCH64_JUMP_SLOT    0000000000000000 strstr + 0
-0000000000012f58  0000001800000402 R_AARCH64_JUMP_SLOT    0000000000000000 read + 0
-0000000000012f60  0000001900000402 R_AARCH64_JUMP_SLOT    0000000000000000 strncpy + 0
-0000000000012f68  0000001a00000402 R_AARCH64_JUMP_SLOT    0000000000000000 __cxa_atexit + 0
-0000000000012f70  0000001b00000402 R_AARCH64_JUMP_SLOT    0000000000000000 strtok + 0
-0000000000012f78  0000001c00000402 R_AARCH64_JUMP_SLOT    0000000000000000 dlsym + 0
-0000000000012f80  0000001e00000402 R_AARCH64_JUMP_SLOT    0000000000000000 fopen + 0
-0000000000012f88  0000002000000402 R_AARCH64_JUMP_SLOT    0000000000000000 memset + 0
-0000000000012f90  0000002100000402 R_AARCH64_JUMP_SLOT    0000000000000000 fclose + 0
-0000000000012f98  0000002400000402 R_AARCH64_JUMP_SLOT    0000000000000000 strcmp + 0
-0000000000012fa0  0000002600000402 R_AARCH64_JUMP_SLOT    0000000000000000 sprintf + 0
-0000000000012fa8  0000002700000402 R_AARCH64_JUMP_SLOT    0000000000000000 fputc + 0
-0000000000012fb0  0000002800000402 R_AARCH64_JUMP_SLOT    0000000000000000 stat + 0
-0000000000012fb8  0000002900000402 R_AARCH64_JUMP_SLOT    0000000000000000 access + 0
-0000000000012fc0  0000002e00000402 R_AARCH64_JUMP_SLOT    0000000000000000 open + 0
-0000000000012fc8  0000002f00000402 R_AARCH64_JUMP_SLOT    0000000000000000 setsid + 0
-0000000000012fd0  0000003200000402 R_AARCH64_JUMP_SLOT    0000000000000000 mkdir + 0
-0000000000012fd8  0000003300000402 R_AARCH64_JUMP_SLOT    0000000000000000 close + 0
-0000000000012fe0  0000003400000402 R_AARCH64_JUMP_SLOT    0000000000000000 free + 0
+0000000000012ea0  0000000300000402 R_AARCH64_JUMP_SLOT    0000000000000000 atoi@LIBC + 0
+0000000000012ea8  0000000400000402 R_AARCH64_JUMP_SLOT    0000000000000000 pthread_create@LIBC + 0
+0000000000012eb0  0000000600000402 R_AARCH64_JUMP_SLOT    0000000000000000 open@LIBC + 0
+0000000000012eb8  0000000700000402 R_AARCH64_JUMP_SLOT    0000000000000000 umask@LIBC + 0
+0000000000012ec0  0000000800000402 R_AARCH64_JUMP_SLOT    0000000000000000 __cxa_finalize@LIBC + 0
+0000000000012ec8  0000000900000402 R_AARCH64_JUMP_SLOT    0000000000000000 mkdir@LIBC + 0
+0000000000012ed0  0000000a00000402 R_AARCH64_JUMP_SLOT    0000000000000000 read@LIBC + 0
+0000000000012ed8  0000000b00000402 R_AARCH64_JUMP_SLOT    0000000000002174 setApiBlacklistExemptions + 0
+0000000000012ee0  0000000c00000402 R_AARCH64_JUMP_SLOT    0000000000000000 strtoul@LIBC + 0
+0000000000012ee8  0000000d00000402 R_AARCH64_JUMP_SLOT    0000000000000000 fstat@LIBC + 0
+0000000000012ef0  0000000e00000402 R_AARCH64_JUMP_SLOT    0000000000000000 chmod@LIBC + 0
+0000000000012ef8  0000000f00000402 R_AARCH64_JUMP_SLOT    0000000000000000 setsid@LIBC + 0
+0000000000012f00  0000001000000402 R_AARCH64_JUMP_SLOT    0000000000001b28 get_file_size + 0
+0000000000012f08  0000001200000402 R_AARCH64_JUMP_SLOT    0000000000000000 access@LIBC + 0
+0000000000012f10  0000001300000402 R_AARCH64_JUMP_SLOT    0000000000000000 fclose@LIBC + 0
+0000000000012f18  0000001400000402 R_AARCH64_JUMP_SLOT    0000000000000000 fputc@LIBC + 0
+0000000000012f20  0000001500000402 R_AARCH64_JUMP_SLOT    0000000000000000 __stack_chk_fail@LIBC + 0
+0000000000012f28  0000001600000402 R_AARCH64_JUMP_SLOT    0000000000000000 fgets@LIBC + 0
+0000000000012f30  0000001700000402 R_AARCH64_JUMP_SLOT    0000000000000000 getc@LIBC + 0
+0000000000012f38  0000001800000402 R_AARCH64_JUMP_SLOT    0000000000001b7c copyfile + 0
+0000000000012f40  0000001900000402 R_AARCH64_JUMP_SLOT    0000000000001c60 get_module_base + 0
+0000000000012f48  0000001b00000402 R_AARCH64_JUMP_SLOT    0000000000000000 strncpy@LIBC + 0
+0000000000012f50  0000001c00000402 R_AARCH64_JUMP_SLOT    0000000000000000 dlsym@LIBC + 0
+0000000000012f58  0000001e00000402 R_AARCH64_JUMP_SLOT    0000000000000000 __android_log_print + 0
+0000000000012f60  0000002000000402 R_AARCH64_JUMP_SLOT    0000000000000000 strcmp@LIBC + 0
+0000000000012f68  0000002100000402 R_AARCH64_JUMP_SLOT    0000000000000000 sprintf@LIBC + 0
+0000000000012f70  0000002200000402 R_AARCH64_JUMP_SLOT    0000000000000000 mmap@LIBC + 0
+0000000000012f78  0000002300000402 R_AARCH64_JUMP_SLOT    0000000000001d2c get_symbol_offset + 0
+0000000000012f80  0000002500000402 R_AARCH64_JUMP_SLOT    0000000000001ac0 get_sdk_version + 0
+0000000000012f88  0000002600000402 R_AARCH64_JUMP_SLOT    0000000000000000 getuid@LIBC + 0
+0000000000012f90  0000002700000402 R_AARCH64_JUMP_SLOT    0000000000000000 strstr@LIBC + 0
+0000000000012f98  0000002800000402 R_AARCH64_JUMP_SLOT    0000000000000000 strtok@LIBC + 0
+0000000000012fa0  0000002a00000402 R_AARCH64_JUMP_SLOT    0000000000000000 close@LIBC + 0
+0000000000012fa8  0000002c00000402 R_AARCH64_JUMP_SLOT    0000000000000000 stat@LIBC + 0
+0000000000012fb0  0000002e00000402 R_AARCH64_JUMP_SLOT    0000000000000000 munmap@LIBC + 0
+0000000000012fb8  0000003000000402 R_AARCH64_JUMP_SLOT    0000000000000000 malloc@LIBC + 0
+0000000000012fc0  0000003200000402 R_AARCH64_JUMP_SLOT    0000000000000000 memset@LIBC + 0
+0000000000012fc8  0000003300000402 R_AARCH64_JUMP_SLOT    0000000000000000 fopen@LIBC + 0
+0000000000012fd0  0000003500000402 R_AARCH64_JUMP_SLOT    0000000000000000 free@LIBC + 0
+0000000000012fd8  0000003600000402 R_AARCH64_JUMP_SLOT    0000000000000000 __system_property_get@LIBC + 0
+0000000000012fe0  0000003700000402 R_AARCH64_JUMP_SLOT    0000000000002044 get_jni_env + 0
+0000000000012fe8  0000003800000402 R_AARCH64_JUMP_SLOT    0000000000000000 __cxa_atexit@LIBC + 0
```

#### readelf --wide --dynamic {}

```diff
@@ -1,30 +1,32 @@
 
-Dynamic section at offset 0x2cd8 contains 27 entries:
+Dynamic section at offset 0x2c78 contains 29 entries:
   Tag        Type                         Name/Value
  0x0000000000000001 (NEEDED)             Shared library: [liblog.so]
- 0x0000000000000001 (NEEDED)             Shared library: [libstdc++.so]
- 0x0000000000000001 (NEEDED)             Shared library: [libm.so]
  0x0000000000000001 (NEEDED)             Shared library: [libc.so]
+ 0x0000000000000001 (NEEDED)             Shared library: [libm.so]
+ 0x0000000000000001 (NEEDED)             Shared library: [libstdc++.so]
  0x0000000000000001 (NEEDED)             Shared library: [libdl.so]
  0x000000000000000e (SONAME)             Library soname: [libdexloader.so]
- 0x0000000000000010 (SYMBOLIC)           0x0
- 0x0000000000000019 (INIT_ARRAY)         0x12cc0
+ 0x0000000000000019 (INIT_ARRAY)         0x12c60
  0x000000000000001b (INIT_ARRAYSZ)       8 (bytes)
- 0x000000000000001a (FINI_ARRAY)         0x12cc8
+ 0x000000000000001a (FINI_ARRAY)         0x12c68
  0x000000000000001c (FINI_ARRAYSZ)       16 (bytes)
- 0x0000000000000004 (HASH)               0x190
- 0x0000000000000005 (STRTAB)             0x7f8
- 0x0000000000000006 (SYMTAB)             0x300
- 0x000000000000000a (STRSZ)              572 (bytes)
+ 0x0000000000000004 (HASH)               0x228
+ 0x0000000000000005 (STRTAB)             0x900
+ 0x0000000000000006 (SYMTAB)             0x3a8
+ 0x000000000000000a (STRSZ)              639 (bytes)
  0x000000000000000b (SYMENT)             24 (bytes)
- 0x0000000000000003 (PLTGOT)             0x12ec8
- 0x0000000000000002 (PLTRELSZ)           792 (bytes)
+ 0x0000000000000003 (PLTGOT)             0x12e88
+ 0x0000000000000002 (PLTRELSZ)           1008 (bytes)
  0x0000000000000014 (PLTREL)             RELA
- 0x0000000000000017 (JMPREL)             0xa80
- 0x0000000000000007 (RELA)               0xa38
- 0x0000000000000008 (RELASZ)             72 (bytes)
+ 0x0000000000000017 (JMPREL)             0xc68
+ 0x0000000000000007 (RELA)               0xc38
+ 0x0000000000000008 (RELASZ)             48 (bytes)
  0x0000000000000009 (RELAENT)            24 (bytes)
  0x0000000000000018 (BIND_NOW)           
  0x000000006ffffffb (FLAGS_1)            Flags: NOW
- 0x000000006ffffff9 (RELACOUNT)          2
+ 0x000000006ffffffe (VERNEED)            0xbf8
+ 0x000000006fffffff (VERNEEDNUM)         2
+ 0x000000006ffffff0 (VERSYM)             0xb80
+ 0x000000006ffffff9 (RELACOUNT)          1
  0x0000000000000000 (NULL)               0x0
```

#### readelf --wide --notes {}

```diff
@@ -0,0 +1,8 @@
+
+Displaying notes found in: .note.gnu.build-id
+  Owner                Data size 	Description
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 41459d84bb5730a6c939041ae62a13f67e036cdc
+
+Displaying notes found in: .note.android.ident
+  Owner                Data size 	Description
+  Android              0x00000084	NT_VERSION (version)	   description data: 15 00 00 00 72 31 36 62 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 34 34 37 39 34 39 39 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00
```

#### readelf --wide --version-info {}

```diff
@@ -1,2 +1,25 @@
 
-No version information found in this file.
+Version symbols section '.gnu.version' contains 57 entries:
+ Addr: 0x0000000000000b80  Offset: 0x00000b80  Link: 3 (.dynsym)
+  000:   0 (*local*)       0 (*local*)       0 (*local*)       2 (LIBC)       
+  004:   2 (LIBC)          1 (*global*)      2 (LIBC)          2 (LIBC)       
+  008:   2 (LIBC)          2 (LIBC)          2 (LIBC)          1 (*global*)   
+  00c:   2 (LIBC)          2 (LIBC)          2 (LIBC)          2 (LIBC)       
+  010:   1 (*global*)      1 (*global*)      2 (LIBC)          2 (LIBC)       
+  014:   2 (LIBC)          2 (LIBC)          2 (LIBC)          2 (LIBC)       
+  018:   1 (*global*)      1 (*global*)      1 (*global*)      2 (LIBC)       
+  01c:   3 (LIBC)          1 (*global*)      0 (*local*)       1 (*global*)   
+  020:   2 (LIBC)          2 (LIBC)          2 (LIBC)          1 (*global*)   
+  024:   1 (*global*)      1 (*global*)      2 (LIBC)          2 (LIBC)       
+  028:   2 (LIBC)          1 (*global*)      2 (LIBC)          1 (*global*)   
+  02c:   2 (LIBC)          1 (*global*)      2 (LIBC)          1 (*global*)   
+  030:   2 (LIBC)          1 (*global*)      2 (LIBC)          2 (LIBC)       
+  034:   1 (*global*)      2 (LIBC)          2 (LIBC)          1 (*global*)   
+  038:   2 (LIBC)       
+
+Version needs section '.gnu.version_r' contains 2 entries:
+ Addr: 0x0000000000000bf8  Offset: 0x00000bf8  Link: 4 (.dynstr)
+  000000: Version: 1  File: libdl.so  Cnt: 1
+  0x0010:   Name: LIBC  Flags: none  Version: 3
+  0x0020: Version: 1  File: libc.so  Cnt: 1
+  0x0030:   Name: LIBC  Flags: none  Version: 2
```

#### readelf --wide --debug-dump=frames {}

```diff
@@ -1,282 +1,178 @@
 Contents of the .eh_frame section:
 
 
 00000000 0000000000000014 00000000 CIE
   Version:               1
   Augmentation:          "zR"
-  Code alignment factor: 4
-  Data alignment factor: -8
+  Code alignment factor: 1
+  Data alignment factor: -4
   Return address column: 30
   Augmentation data:     1b
   DW_CFA_def_cfa: r31 (sp) ofs 0
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000018 000000000000003c 0000001c FDE cie=00000000 pc=000000000000100c..0000000000001364
-  DW_CFA_advance_loc: 4 to 0000000000001010
-  DW_CFA_def_cfa_offset: 96
-  DW_CFA_advance_loc: 12 to 000000000000101c
-  DW_CFA_offset: r21 (x21) at cfa-80
-  DW_CFA_offset: r22 (x22) at cfa-72
-  DW_CFA_advance_loc: 16 to 000000000000102c
-  DW_CFA_offset: r19 (x19) at cfa-96
-  DW_CFA_offset: r20 (x20) at cfa-88
-  DW_CFA_offset: r23 (x23) at cfa-64
-  DW_CFA_offset: r24 (x24) at cfa-56
-  DW_CFA_advance_loc: 8 to 0000000000001034
-  DW_CFA_offset: r25 (x25) at cfa-48
-  DW_CFA_offset: r30 (x30) at cfa-40
-  DW_CFA_advance_loc1: 628 to 00000000000012a8
-  DW_CFA_remember_state
-  DW_CFA_restore: r20 (x20)
-  DW_CFA_restore: r19 (x19)
-  DW_CFA_advance_loc: 4 to 00000000000012ac
-  DW_CFA_restore: r22 (x22)
-  DW_CFA_restore: r21 (x21)
-  DW_CFA_advance_loc: 4 to 00000000000012b0
-  DW_CFA_restore: r24 (x24)
-  DW_CFA_restore: r23 (x23)
-  DW_CFA_advance_loc: 4 to 00000000000012b4
-  DW_CFA_restore: r30 (x30)
-  DW_CFA_restore: r25 (x25)
-  DW_CFA_advance_loc: 4 to 00000000000012b8
-  DW_CFA_def_cfa_offset: 0
-  DW_CFA_advance_loc: 4 to 00000000000012bc
-  DW_CFA_restore_state
+00000018 0000000000000024 0000001c FDE cie=00000000 pc=000000000000135c..00000000000016dc
+  DW_CFA_advance_loc: 28 to 0000000000001378
+  DW_CFA_def_cfa: r29 (x29) ofs 16
+  DW_CFA_offset: r30 (x30) at cfa-8
+  DW_CFA_offset: r29 (x29) at cfa-16
+  DW_CFA_offset: r19 (x19) at cfa-24
+  DW_CFA_offset: r20 (x20) at cfa-32
+  DW_CFA_offset: r21 (x21) at cfa-40
+  DW_CFA_offset: r22 (x22) at cfa-48
+  DW_CFA_offset: r23 (x23) at cfa-56
+  DW_CFA_offset: r24 (x24) at cfa-64
+  DW_CFA_offset: r25 (x25) at cfa-80
   DW_CFA_nop
+
+00000040 000000000000002c 00000044 FDE cie=00000000 pc=00000000000016dc..00000000000019c8
+  DW_CFA_advance_loc: 32 to 00000000000016fc
+  DW_CFA_def_cfa: r29 (x29) ofs 16
+  DW_CFA_offset: r30 (x30) at cfa-8
+  DW_CFA_offset: r29 (x29) at cfa-16
+  DW_CFA_offset: r19 (x19) at cfa-24
+  DW_CFA_offset: r20 (x20) at cfa-32
+  DW_CFA_offset: r21 (x21) at cfa-40
+  DW_CFA_offset: r22 (x22) at cfa-48
+  DW_CFA_offset: r23 (x23) at cfa-56
+  DW_CFA_offset: r24 (x24) at cfa-64
+  DW_CFA_offset: r25 (x25) at cfa-72
+  DW_CFA_offset: r26 (x26) at cfa-80
+  DW_CFA_offset: r28 (x28) at cfa-96
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000058 000000000000004c 0000005c FDE cie=00000000 pc=0000000000001364..00000000000016a0
-  DW_CFA_advance_loc: 4 to 0000000000001368
-  DW_CFA_def_cfa_offset: 832
-  DW_CFA_advance_loc: 4 to 000000000000136c
-  DW_CFA_def_cfa_offset: 928
-  DW_CFA_advance_loc: 4 to 0000000000001370
-  DW_CFA_offset: r21 (x21) at cfa-912
-  DW_CFA_offset: r22 (x22) at cfa-904
-  DW_CFA_advance_loc: 20 to 0000000000001384
-  DW_CFA_offset: r30 (x30) at cfa-848
-  DW_CFA_offset: r23 (x23) at cfa-896
-  DW_CFA_offset: r24 (x24) at cfa-888
-  DW_CFA_offset: r25 (x25) at cfa-880
-  DW_CFA_offset: r26 (x26) at cfa-872
-  DW_CFA_advance_loc: 12 to 0000000000001390
-  DW_CFA_offset: r19 (x19) at cfa-928
-  DW_CFA_offset: r20 (x20) at cfa-920
-  DW_CFA_offset: r27 (x27) at cfa-864
-  DW_CFA_offset: r28 (x28) at cfa-856
-  DW_CFA_advance_loc1: 632 to 0000000000001608
-  DW_CFA_remember_state
-  DW_CFA_restore: r20 (x20)
-  DW_CFA_restore: r19 (x19)
-  DW_CFA_advance_loc: 4 to 000000000000160c
-  DW_CFA_restore: r22 (x22)
-  DW_CFA_restore: r21 (x21)
-  DW_CFA_advance_loc: 4 to 0000000000001610
-  DW_CFA_restore: r24 (x24)
-  DW_CFA_restore: r23 (x23)
-  DW_CFA_advance_loc: 4 to 0000000000001614
-  DW_CFA_restore: r26 (x26)
-  DW_CFA_restore: r25 (x25)
-  DW_CFA_advance_loc: 4 to 0000000000001618
-  DW_CFA_restore: r28 (x28)
-  DW_CFA_restore: r27 (x27)
-  DW_CFA_advance_loc: 4 to 000000000000161c
-  DW_CFA_restore: r30 (x30)
-  DW_CFA_advance_loc: 4 to 0000000000001620
-  DW_CFA_def_cfa_offset: 832
-  DW_CFA_advance_loc: 4 to 0000000000001624
-  DW_CFA_def_cfa_offset: 736
-  DW_CFA_advance_loc: 4 to 0000000000001628
-  DW_CFA_restore_state
-  DW_CFA_nop
-
-000000a8 0000000000000014 000000ac FDE cie=00000000 pc=00000000000016a0..00000000000016a4
+00000070 0000000000000014 00000074 FDE cie=00000000 pc=00000000000019c8..00000000000019cc
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000000c0 000000000000001c 000000c4 FDE cie=00000000 pc=00000000000016a4..00000000000016c4
-  DW_CFA_advance_loc: 4 to 00000000000016a8
-  DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 8 to 00000000000016b0
-  DW_CFA_offset: r30 (x30) at cfa-16
-  DW_CFA_advance_loc: 12 to 00000000000016bc
-  DW_CFA_restore: r30 (x30)
-  DW_CFA_advance_loc: 4 to 00000000000016c0
-  DW_CFA_def_cfa_offset: 0
+00000088 000000000000001c 0000008c FDE cie=00000000 pc=00000000000019cc..00000000000019e8
+  DW_CFA_advance_loc: 8 to 00000000000019d4
+  DW_CFA_def_cfa: r29 (x29) ofs 16
+  DW_CFA_offset: r30 (x30) at cfa-8
+  DW_CFA_offset: r29 (x29) at cfa-16
+  DW_CFA_nop
+  DW_CFA_nop
+  DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000000e0 0000000000000024 000000e4 FDE cie=00000000 pc=00000000000016c4..0000000000001710
-  DW_CFA_advance_loc: 4 to 00000000000016c8
-  DW_CFA_def_cfa_offset: 160
-  DW_CFA_advance_loc: 8 to 00000000000016d0
-  DW_CFA_offset: r19 (x19) at cfa-160
-  DW_CFA_offset: r30 (x30) at cfa-152
-  DW_CFA_advance_loc: 52 to 0000000000001704
-  DW_CFA_remember_state
-  DW_CFA_restore: r30 (x30)
-  DW_CFA_restore: r19 (x19)
-  DW_CFA_advance_loc: 4 to 0000000000001708
-  DW_CFA_def_cfa_offset: 0
-  DW_CFA_advance_loc: 4 to 000000000000170c
-  DW_CFA_restore_state
+000000a8 000000000000001c 000000ac FDE cie=00000000 pc=00000000000019e8..0000000000001ac0
+  DW_CFA_advance_loc: 20 to 00000000000019fc
+  DW_CFA_def_cfa: r29 (x29) ofs 16
+  DW_CFA_offset: r30 (x30) at cfa-8
+  DW_CFA_offset: r29 (x29) at cfa-16
+  DW_CFA_offset: r19 (x19) at cfa-24
+  DW_CFA_offset: r20 (x20) at cfa-32
+  DW_CFA_offset: r21 (x21) at cfa-48
+  DW_CFA_nop
+
+000000c8 000000000000001c 000000cc FDE cie=00000000 pc=0000000000001ac0..0000000000001b28
+  DW_CFA_advance_loc: 16 to 0000000000001ad0
+  DW_CFA_def_cfa: r29 (x29) ofs 16
+  DW_CFA_offset: r30 (x30) at cfa-8
+  DW_CFA_offset: r29 (x29) at cfa-16
+  DW_CFA_offset: r19 (x19) at cfa-32
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000108 000000000000002c 0000010c FDE cie=00000000 pc=0000000000001710..0000000000001800
-  DW_CFA_advance_loc: 4 to 0000000000001714
-  DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 16 to 0000000000001724
-  DW_CFA_offset: r21 (x21) at cfa-32
-  DW_CFA_offset: r22 (x22) at cfa-24
-  DW_CFA_advance_loc: 24 to 000000000000173c
-  DW_CFA_offset: r19 (x19) at cfa-48
-  DW_CFA_offset: r20 (x20) at cfa-40
-  DW_CFA_advance_loc: 12 to 0000000000001748
-  DW_CFA_offset: r30 (x30) at cfa-16
-  DW_CFA_advance_loc: 104 to 00000000000017b0
-  DW_CFA_remember_state
-  DW_CFA_restore: r20 (x20)
-  DW_CFA_restore: r19 (x19)
-  DW_CFA_advance_loc: 4 to 00000000000017b4
-  DW_CFA_restore: r22 (x22)
-  DW_CFA_restore: r21 (x21)
-  DW_CFA_advance_loc: 4 to 00000000000017b8
-  DW_CFA_restore: r30 (x30)
-  DW_CFA_advance_loc: 4 to 00000000000017bc
-  DW_CFA_def_cfa_offset: 0
-  DW_CFA_advance_loc: 4 to 00000000000017c0
-  DW_CFA_restore_state
-  DW_CFA_nop
-
-00000138 000000000000003c 0000013c FDE cie=00000000 pc=0000000000001800..00000000000018e4
-  DW_CFA_advance_loc: 4 to 0000000000001804
-  DW_CFA_def_cfa_offset: 1040
-  DW_CFA_advance_loc: 8 to 000000000000180c
-  DW_CFA_def_cfa_offset: 1088
-  DW_CFA_advance_loc: 8 to 0000000000001814
-  DW_CFA_offset: r21 (x21) at cfa-1072
-  DW_CFA_offset: r22 (x22) at cfa-1064
-  DW_CFA_advance_loc: 12 to 0000000000001820
-  DW_CFA_offset: r30 (x30) at cfa-1056
-  DW_CFA_offset: r19 (x19) at cfa-1088
-  DW_CFA_offset: r20 (x20) at cfa-1080
-  DW_CFA_advance_loc: 120 to 0000000000001898
-  DW_CFA_remember_state
-  DW_CFA_restore: r20 (x20)
-  DW_CFA_restore: r19 (x19)
-  DW_CFA_advance_loc: 4 to 000000000000189c
-  DW_CFA_restore: r22 (x22)
-  DW_CFA_restore: r21 (x21)
-  DW_CFA_advance_loc: 4 to 00000000000018a0
-  DW_CFA_restore: r30 (x30)
-  DW_CFA_advance_loc: 4 to 00000000000018a4
-  DW_CFA_def_cfa_offset: 1040
-  DW_CFA_advance_loc: 4 to 00000000000018a8
-  DW_CFA_def_cfa_offset: 992
-  DW_CFA_advance_loc: 4 to 00000000000018ac
-  DW_CFA_restore_state
-  DW_CFA_nop
-  DW_CFA_nop
-  DW_CFA_nop
-
-00000178 000000000000003c 0000017c FDE cie=00000000 pc=00000000000018e4..0000000000001c18
-  DW_CFA_advance_loc: 4 to 00000000000018e8
-  DW_CFA_def_cfa_offset: 224
-  DW_CFA_advance_loc: 4 to 00000000000018ec
-  DW_CFA_offset: r19 (x19) at cfa-224
-  DW_CFA_offset: r20 (x20) at cfa-216
-  DW_CFA_advance_loc: 20 to 0000000000001900
-  DW_CFA_offset: r30 (x30) at cfa-160
-  DW_CFA_offset: r21 (x21) at cfa-208
-  DW_CFA_offset: r22 (x22) at cfa-200
-  DW_CFA_offset: r23 (x23) at cfa-192
-  DW_CFA_offset: r24 (x24) at cfa-184
-  DW_CFA_advance_loc: 8 to 0000000000001908
-  DW_CFA_offset: r25 (x25) at cfa-176
-  DW_CFA_offset: r26 (x26) at cfa-168
-  DW_CFA_advance_loc1: 600 to 0000000000001b60
-  DW_CFA_remember_state
-  DW_CFA_restore: r20 (x20)
-  DW_CFA_restore: r19 (x19)
-  DW_CFA_advance_loc: 4 to 0000000000001b64
-  DW_CFA_restore: r22 (x22)
-  DW_CFA_restore: r21 (x21)
-  DW_CFA_advance_loc: 4 to 0000000000001b68
-  DW_CFA_restore: r24 (x24)
-  DW_CFA_restore: r23 (x23)
-  DW_CFA_advance_loc: 4 to 0000000000001b6c
-  DW_CFA_restore: r26 (x26)
-  DW_CFA_restore: r25 (x25)
-  DW_CFA_advance_loc: 4 to 0000000000001b70
-  DW_CFA_restore: r30 (x30)
-  DW_CFA_advance_loc: 4 to 0000000000001b74
-  DW_CFA_def_cfa_offset: 0
-  DW_CFA_advance_loc: 4 to 0000000000001b78
-  DW_CFA_restore_state
-  DW_CFA_nop
-
-000001b8 0000000000000044 000001bc FDE cie=00000000 pc=0000000000001c18..0000000000001d4c
-  DW_CFA_advance_loc: 4 to 0000000000001c1c
-  DW_CFA_def_cfa_offset: 64
-  DW_CFA_advance_loc: 8 to 0000000000001c24
-  DW_CFA_offset: r19 (x19) at cfa-64
-  DW_CFA_offset: r20 (x20) at cfa-56
-  DW_CFA_advance_loc: 24 to 0000000000001c3c
-  DW_CFA_offset: r30 (x30) at cfa-16
+000000e8 000000000000001c 000000ec FDE cie=00000000 pc=0000000000001b28..0000000000001b7c
+  DW_CFA_advance_loc: 16 to 0000000000001b38
+  DW_CFA_def_cfa: r29 (x29) ofs 16
+  DW_CFA_offset: r30 (x30) at cfa-8
+  DW_CFA_offset: r29 (x29) at cfa-16
+  DW_CFA_offset: r19 (x19) at cfa-32
+  DW_CFA_nop
+  DW_CFA_nop
+  DW_CFA_nop
+  DW_CFA_nop
+  DW_CFA_nop
+
+00000108 000000000000001c 0000010c FDE cie=00000000 pc=0000000000001b7c..0000000000001c60
+  DW_CFA_advance_loc: 16 to 0000000000001b8c
+  DW_CFA_def_cfa: r29 (x29) ofs 16
+  DW_CFA_offset: r30 (x30) at cfa-8
+  DW_CFA_offset: r29 (x29) at cfa-16
+  DW_CFA_offset: r19 (x19) at cfa-24
+  DW_CFA_offset: r20 (x20) at cfa-32
   DW_CFA_offset: r21 (x21) at cfa-48
-  DW_CFA_offset: r22 (x22) at cfa-40
-  DW_CFA_offset: r23 (x23) at cfa-32
-  DW_CFA_offset: r24 (x24) at cfa-24
-  DW_CFA_advance_loc: 48 to 0000000000001c6c
-  DW_CFA_remember_state
-  DW_CFA_restore: r20 (x20)
-  DW_CFA_restore: r19 (x19)
-  DW_CFA_advance_loc: 4 to 0000000000001c70
-  DW_CFA_restore: r22 (x22)
-  DW_CFA_restore: r21 (x21)
-  DW_CFA_advance_loc: 4 to 0000000000001c74
-  DW_CFA_restore: r24 (x24)
-  DW_CFA_restore: r23 (x23)
-  DW_CFA_advance_loc: 4 to 0000000000001c78
-  DW_CFA_restore: r30 (x30)
-  DW_CFA_advance_loc: 4 to 0000000000001c7c
-  DW_CFA_def_cfa_offset: 0
-  DW_CFA_advance_loc: 4 to 0000000000001c80
-  DW_CFA_restore_state
-  DW_CFA_advance_loc: 120 to 0000000000001cf8
-  DW_CFA_remember_state
-  DW_CFA_restore: r30 (x30)
-  DW_CFA_advance_loc: 4 to 0000000000001cfc
-  DW_CFA_restore: r19 (x19)
-  DW_CFA_restore: r20 (x20)
-  DW_CFA_advance_loc: 4 to 0000000000001d00
-  DW_CFA_restore: r21 (x21)
-  DW_CFA_restore: r22 (x22)
-  DW_CFA_advance_loc: 4 to 0000000000001d04
-  DW_CFA_restore: r23 (x23)
-  DW_CFA_restore: r24 (x24)
-  DW_CFA_advance_loc: 4 to 0000000000001d08
-  DW_CFA_def_cfa_offset: 0
-  DW_CFA_advance_loc: 4 to 0000000000001d0c
-  DW_CFA_restore_state
+  DW_CFA_nop
+
+00000128 0000000000000024 0000012c FDE cie=00000000 pc=0000000000001c60..0000000000001d2c
+  DW_CFA_advance_loc: 20 to 0000000000001c74
+  DW_CFA_def_cfa: r29 (x29) ofs 16
+  DW_CFA_offset: r30 (x30) at cfa-8
+  DW_CFA_offset: r29 (x29) at cfa-16
+  DW_CFA_offset: r19 (x19) at cfa-24
+  DW_CFA_offset: r20 (x20) at cfa-32
+  DW_CFA_offset: r21 (x21) at cfa-40
+  DW_CFA_offset: r28 (x28) at cfa-48
+  DW_CFA_nop
+  DW_CFA_nop
+  DW_CFA_nop
+  DW_CFA_nop
+  DW_CFA_nop
+  DW_CFA_nop
+  DW_CFA_nop
+
+00000150 000000000000002c 00000154 FDE cie=00000000 pc=0000000000001d2c..0000000000002044
+  DW_CFA_advance_loc: 32 to 0000000000001d4c
+  DW_CFA_def_cfa: r29 (x29) ofs 16
+  DW_CFA_offset: r30 (x30) at cfa-8
+  DW_CFA_offset: r29 (x29) at cfa-16
+  DW_CFA_offset: r19 (x19) at cfa-24
+  DW_CFA_offset: r20 (x20) at cfa-32
+  DW_CFA_offset: r21 (x21) at cfa-40
+  DW_CFA_offset: r22 (x22) at cfa-48
+  DW_CFA_offset: r23 (x23) at cfa-56
+  DW_CFA_offset: r24 (x24) at cfa-64
+  DW_CFA_offset: r25 (x25) at cfa-72
+  DW_CFA_offset: r26 (x26) at cfa-80
+  DW_CFA_offset: r27 (x27) at cfa-96
+  DW_CFA_nop
+  DW_CFA_nop
+  DW_CFA_nop
+  DW_CFA_nop
+  DW_CFA_nop
+
+00000180 000000000000001c 00000184 FDE cie=00000000 pc=0000000000002044..0000000000002174
+  DW_CFA_advance_loc: 16 to 0000000000002054
+  DW_CFA_def_cfa: r29 (x29) ofs 16
+  DW_CFA_offset: r30 (x30) at cfa-8
+  DW_CFA_offset: r29 (x29) at cfa-16
+  DW_CFA_offset: r19 (x19) at cfa-24
+  DW_CFA_offset: r20 (x20) at cfa-32
+  DW_CFA_offset: r21 (x21) at cfa-48
+  DW_CFA_nop
+
+000001a0 0000000000000024 000001a4 FDE cie=00000000 pc=0000000000002174..0000000000002348
+  DW_CFA_advance_loc: 20 to 0000000000002188
+  DW_CFA_def_cfa: r29 (x29) ofs 16
+  DW_CFA_offset: r30 (x30) at cfa-8
+  DW_CFA_offset: r29 (x29) at cfa-16
+  DW_CFA_offset: r19 (x19) at cfa-24
+  DW_CFA_offset: r20 (x20) at cfa-32
+  DW_CFA_offset: r21 (x21) at cfa-40
+  DW_CFA_offset: r22 (x22) at cfa-48
+  DW_CFA_offset: r23 (x23) at cfa-56
+  DW_CFA_offset: r24 (x24) at cfa-64
+  DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
```

#### strings --all --bytes=8 {}

```diff
@@ -1,33 +1,37 @@
 __cxa_finalize
 __cxa_atexit
-load_dex_in_thread
-__stack_chk_guard
+JNI_OnLoad
+Java_com_test_androidspy_HelperUtil_nativeSetsid
+Java_com_test_androidspy_HelperUtil_nativeUmask
 __android_log_print
 __stack_chk_fail
-load_dex
+copyfile
 get_file_size
 get_jni_env
+get_sdk_version
+load_dex
+load_dex_in_thread
 pthread_create
-copyfile
-Java_com_test_androidspy_HelperUtil_nativeSetsid
-Java_com_test_androidspy_HelperUtil_nativeUmask
+setApiBlacklistExemptions
+__system_property_get
 get_module_base
 get_symbol_offset
 liblog.so
 libstdc++.so
 libdl.so
 __bss_start
 __bss_start__
 __bss_end__
 libdexloader.so
 dexloader
 Enter thread
 Get env failed
 Current JNIEnv: %p
+Call setApiBlacklistExemptions
 java/lang/ClassLoader
 getSystemClassLoader
 ()Ljava/lang/ClassLoader;
 dalvik/system/DexClassLoader
 (Ljava/lang/String;Ljava/lang/String;Ljava/lang/String;Ljava/lang/ClassLoader;)V
 Object dex_loader: %p
 findClass
@@ -37,32 +41,47 @@
 Exit thread
 Load dex %s to %s, and call %s.%s %s
 Out file dir: %s
 JNIEnv: %p
 Get jvm failed: %d
 JavaVM: %p
 Create loading thread
+JNI_OnLoad
+ERROR: GetEnv failed
+ro.build.version.sdk
 copy %s to %s
 open %s error !
 /proc/self/maps
 cannot open '%s'
 fstat %s failed: %d
 %s size: %d
 Alloc memory failed
 symtab_offset=0x%x symtab_entries=0x%x strtab_offset=0x%x
 _ZN7android14AndroidRuntime9getJNIEnvEv
 getJNIEnv by dlsym: %p
-/system/lib64/libandroid_runtime.so
 Module %s base: %p
 Must run in Android app process
 Function %s offset: 0x%x
 Function %s not found in %s
-GCC: (GNU) 4.9 20140827 (prerelease)
+com/android/internal/os/ZygoteInit
+Class android.os.ZygoteInit not found
+([Ljava/lang/String;)V
+setApiDenylistExemptions
+Method setApiBlacklistExemptions or setApiDenylistExemptions not found
+java/lang/String
+setApiBlacklistExemptions success
+/system/lib64/libandroid_runtime.so
+GCC: (GNU) 4.9.x 20150123 (prerelease)
+Android clang version 5.0.300080  (based on LLVM 5.0.300080)
 .shstrtab
+.note.gnu.build-id
+.gnu.version
+.gnu.version_r
 .rela.dyn
 .rela.plt
 .eh_frame_hdr
 .eh_frame
+.note.android.ident
 .init_array
 .fini_array
 .dynamic
 .comment
```

#### readelf --wide --decompress --hex-dump=.hash {}

```diff
@@ -1,26 +1,27 @@
 
 Hex dump of section '.hash':
-  0x00000190 25000000 35000000 23000000 24000000 %...5...#...$...
-  0x000001a0 00000000 32000000 04000000 2c000000 ....2.......,...
-  0x000001b0 1c000000 0f000000 00000000 00000000 ................
-  0x000001c0 07000000 14000000 1a000000 00000000 ................
-  0x000001d0 1e000000 21000000 33000000 0d000000 ....!...3.......
-  0x000001e0 2a000000 26000000 00000000 2e000000 *...&...........
-  0x000001f0 00000000 0b000000 22000000 00000000 ........".......
-  0x00000200 00000000 31000000 25000000 00000000 ....1...%.......
-  0x00000210 29000000 34000000 27000000 00000000 )...4...'.......
-  0x00000220 00000000 1f000000 1d000000 00000000 ................
-  0x00000230 00000000 00000000 00000000 00000000 ................
-  0x00000240 00000000 00000000 00000000 00000000 ................
-  0x00000250 00000000 00000000 00000000 00000000 ................
-  0x00000260 00000000 0a000000 00000000 00000000 ................
-  0x00000270 09000000 08000000 03000000 05000000 ................
-  0x00000280 0c000000 11000000 16000000 0e000000 ................
-  0x00000290 00000000 00000000 06000000 13000000 ................
-  0x000002a0 00000000 1b000000 19000000 00000000 ................
-  0x000002b0 00000000 00000000 00000000 12000000 ................
-  0x000002c0 00000000 00000000 20000000 00000000 ........ .......
-  0x000002d0 17000000 28000000 15000000 00000000 ....(...........
-  0x000002e0 00000000 18000000 2d000000 2b000000 ........-...+...
-  0x000002f0 10000000 00000000 2f000000 30000000 ......../...0...
+  0x00000228 25000000 39000000 1d000000 20000000 %...9....... ...
+  0x00000238 25000000 09000000 2e000000 23000000 %...........#...
+  0x00000248 1c000000 2d000000 0b000000 00000000 ....-...........
+  0x00000258 16000000 0d000000 38000000 00000000 ........8.......
+  0x00000268 33000000 13000000 2b000000 0c000000 3.......+.......
+  0x00000278 2f000000 21000000 00000000 26000000 /...!.......&...
+  0x00000288 03000000 30000000 37000000 36000000 ....0...7...6...
+  0x00000298 00000000 22000000 10000000 00000000 ...."...........
+  0x000002a8 27000000 35000000 32000000 00000000 '...5...2.......
+  0x000002b8 00000000 1b000000 29000000 00000000 ........).......
+  0x000002c8 00000000 00000000 00000000 00000000 ................
+  0x000002d8 00000000 00000000 00000000 07000000 ................
+  0x000002e8 00000000 06000000 00000000 00000000 ................
+  0x000002f8 00000000 00000000 00000000 00000000 ................
+  0x00000308 00000000 08000000 00000000 00000000 ................
+  0x00000318 12000000 00000000 0e000000 00000000 ................
+  0x00000328 04000000 00000000 1a000000 19000000 ................
+  0x00000338 00000000 0a000000 00000000 17000000 ................
+  0x00000348 00000000 18000000 00000000 1f000000 ................
+  0x00000358 00000000 1e000000 15000000 05000000 ................
+  0x00000368 11000000 0f000000 2a000000 00000000 ........*.......
+  0x00000378 00000000 00000000 2c000000 00000000 ........,.......
+  0x00000388 24000000 14000000 28000000 31000000 $.......(...1...
+  0x00000398 34000000 00000000 00000000 00000000 4...............
```

#### readelf --wide --decompress --hex-dump=.dynstr {}

```diff
@@ -1,39 +1,43 @@
 
 Hex dump of section '.dynstr':
-  0x000007f8 005f5f63 78615f66 696e616c 697a6500 .__cxa_finalize.
-  0x00000808 5f5f6378 615f6174 65786974 006c6f61 __cxa_atexit.loa
-  0x00000818 645f6465 785f696e 5f746872 65616400 d_dex_in_thread.
-  0x00000828 5f5f7374 61636b5f 63686b5f 67756172 __stack_chk_guar
-  0x00000838 64005f5f 616e6472 6f69645f 6c6f675f d.__android_log_
-  0x00000848 7072696e 74006672 6565005f 5f737461 print.free.__sta
-  0x00000858 636b5f63 686b5f66 61696c00 6c6f6164 ck_chk_fail.load
-  0x00000868 5f646578 006d656d 73657400 7374726e _dex.memset.strn
-  0x00000878 63707900 67657475 69640073 7072696e cpy.getuid.sprin
-  0x00000888 74660061 63636573 73006765 745f6669 tf.access.get_fi
-  0x00000898 6c655f73 697a6500 6765745f 6a6e695f le_size.get_jni_
-  0x000008a8 656e7600 6d616c6c 6f630070 74687265 env.malloc.pthre
-  0x000008b8 61645f63 72656174 65006368 6d6f6400 ad_create.chmod.
-  0x000008c8 636f7079 66696c65 006d6b64 6972004a copyfile.mkdir.J
-  0x000008d8 6176615f 636f6d5f 74657374 5f616e64 ava_com_test_and
-  0x000008e8 726f6964 7370795f 48656c70 65725574 roidspy_HelperUt
-  0x000008f8 696c5f6e 61746976 65536574 73696400 il_nativeSetsid.
-  0x00000908 73657473 6964004a 6176615f 636f6d5f setsid.Java_com_
-  0x00000918 74657374 5f616e64 726f6964 7370795f test_androidspy_
-  0x00000928 48656c70 65725574 696c5f6e 61746976 HelperUtil_nativ
-  0x00000938 65556d61 736b0075 6d61736b 00666f70 eUmask.umask.fop
-  0x00000948 656e0066 70757463 00676574 63006663 en.fputc.getc.fc
-  0x00000958 6c6f7365 00676574 5f6d6f64 756c655f lose.get_module_
-  0x00000968 62617365 00737472 73747200 66676574 base.strstr.fget
-  0x00000978 73007374 72746f6b 00737472 746f756c s.strtok.strtoul
-  0x00000988 00676574 5f73796d 626f6c5f 6f666673 .get_symbol_offs
-  0x00000998 65740066 73746174 006d6d61 70007374 et.fstat.mmap.st
-  0x000009a8 72636d70 006d756e 6d617000 646c7379 rcmp.munmap.dlsy
-  0x000009b8 6d006c69 626c6f67 2e736f00 6c696273 m.liblog.so.libs
-  0x000009c8 7464632b 2b2e736f 006c6962 6d2e736f tdc++.so.libm.so
-  0x000009d8 006c6962 632e736f 006c6962 646c2e73 .libc.so.libdl.s
-  0x000009e8 6f005f65 64617461 005f5f62 73735f73 o._edata.__bss_s
-  0x000009f8 74617274 005f5f62 73735f73 74617274 tart.__bss_start
-  0x00000a08 5f5f005f 5f627373 5f656e64 5f5f005f __.__bss_end__._
-  0x00000a18 5f656e64 5f5f005f 656e6400 6c696264 _end__._end.libd
-  0x00000a28 65786c6f 61646572 2e736f00          exloader.so.
+  0x00000900 005f5f63 78615f66 696e616c 697a6500 .__cxa_finalize.
+  0x00000910 5f5f6378 615f6174 65786974 004a4e49 __cxa_atexit.JNI
+  0x00000920 5f4f6e4c 6f616400 4a617661 5f636f6d _OnLoad.Java_com
+  0x00000930 5f746573 745f616e 64726f69 64737079 _test_androidspy
+  0x00000940 5f48656c 70657255 74696c5f 6e617469 _HelperUtil_nati
+  0x00000950 76655365 74736964 004a6176 615f636f veSetsid.Java_co
+  0x00000960 6d5f7465 73745f61 6e64726f 69647370 m_test_androidsp
+  0x00000970 795f4865 6c706572 5574696c 5f6e6174 y_HelperUtil_nat
+  0x00000980 69766555 6d61736b 005f5f61 6e64726f iveUmask.__andro
+  0x00000990 69645f6c 6f675f70 72696e74 005f5f73 id_log_print.__s
+  0x000009a0 7461636b 5f63686b 5f666169 6c006163 tack_chk_fail.ac
+  0x000009b0 63657373 0063686d 6f640063 6f707966 cess.chmod.copyf
+  0x000009c0 696c6500 66726565 00676574 5f66696c ile.free.get_fil
+  0x000009d0 655f7369 7a650067 65745f6a 6e695f65 e_size.get_jni_e
+  0x000009e0 6e760067 65745f73 646b5f76 65727369 nv.get_sdk_versi
+  0x000009f0 6f6e0067 65747569 64006c6f 61645f64 on.getuid.load_d
+  0x00000a00 6578006c 6f61645f 6465785f 696e5f74 ex.load_dex_in_t
+  0x00000a10 68726561 64006d61 6c6c6f63 006d656d hread.malloc.mem
+  0x00000a20 73657400 6d6b6469 72007074 68726561 set.mkdir.pthrea
+  0x00000a30 645f6372 65617465 00736574 41706942 d_create.setApiB
+  0x00000a40 6c61636b 6c697374 4578656d 7074696f lacklistExemptio
+  0x00000a50 6e730073 65747369 64007370 72696e74 ns.setsid.sprint
+  0x00000a60 66007374 726e6370 7900756d 61736b00 f.strncpy.umask.
+  0x00000a70 5f5f7379 7374656d 5f70726f 70657274 __system_propert
+  0x00000a80 795f6765 74006174 6f690064 6c73796d y_get.atoi.dlsym
+  0x00000a90 0066636c 6f736500 66676574 7300666f .fclose.fgets.fo
+  0x00000aa0 70656e00 66707574 63006673 74617400 pen.fputc.fstat.
+  0x00000ab0 6765745f 6d6f6475 6c655f62 61736500 get_module_base.
+  0x00000ac0 6765745f 73796d62 6f6c5f6f 66667365 get_symbol_offse
+  0x00000ad0 74006765 7463006d 6d617000 6d756e6d t.getc.mmap.munm
+  0x00000ae0 61700073 7472636d 70007374 72737472 ap.strcmp.strstr
+  0x00000af0 00737472 746f6b00 73747274 6f756c00 .strtok.strtoul.
+  0x00000b00 6c69626c 6f672e73 6f006c69 62632e73 liblog.so.libc.s
+  0x00000b10 6f006c69 626d2e73 6f006c69 62737464 o.libm.so.libstd
+  0x00000b20 632b2b2e 736f006c 6962646c 2e736f00 c++.so.libdl.so.
+  0x00000b30 5f656461 7461005f 5f627373 5f737461 _edata.__bss_sta
+  0x00000b40 7274005f 5f627373 5f737461 72745f5f rt.__bss_start__
+  0x00000b50 005f5f62 73735f65 6e645f5f 005f5f65 .__bss_end__.__e
+  0x00000b60 6e645f5f 005f656e 64006c69 62646578 nd__._end.libdex
+  0x00000b70 6c6f6164 65722e73 6f004c49 424300   loader.so.LIBC.
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.plt {}

```diff
@@ -1,212 +1,266 @@
 
 
 
 Disassembly of section .plt:
 
-0000000000000da0 <pthread_create@plt-0x20>:
+0000000000001060 <atoi@plt-0x20>:
 	stp	x16, x30, [sp, #-16]!
-	adrp	x16, 12000 <get_jni_env+0x103e8>
-	ldr	x17, [x16, #3800]
-	add	x16, x16, #0xed8
+	adrp	x16, 12000 <setApiBlacklistExemptions@@Base+0xfe8c>
+	ldr	x17, [x16, #3736]
+	add	x16, x16, #0xe98
 	br	x17
 	nop
 	nop
 	nop
 
-0000000000000dc0 <pthread_create@plt>:
-	adrp	x16, 12000 <get_jni_env+0x103e8>
+0000000000001080 <atoi@plt>:
+	adrp	x16, 12000 <setApiBlacklistExemptions@@Base+0xfe8c>
+	ldr	x17, [x16, #3744]
+	add	x16, x16, #0xea0
+	br	x17
+
+0000000000001090 <pthread_create@plt>:
+	adrp	x16, 12000 <setApiBlacklistExemptions@@Base+0xfe8c>
+	ldr	x17, [x16, #3752]
+	add	x16, x16, #0xea8
+	br	x17
+
+00000000000010a0 <open@plt>:
+	adrp	x16, 12000 <setApiBlacklistExemptions@@Base+0xfe8c>
+	ldr	x17, [x16, #3760]
+	add	x16, x16, #0xeb0
+	br	x17
+
+00000000000010b0 <umask@plt>:
+	adrp	x16, 12000 <setApiBlacklistExemptions@@Base+0xfe8c>
+	ldr	x17, [x16, #3768]
+	add	x16, x16, #0xeb8
+	br	x17
+
+00000000000010c0 <__cxa_finalize@plt>:
+	adrp	x16, 12000 <setApiBlacklistExemptions@@Base+0xfe8c>
+	ldr	x17, [x16, #3776]
+	add	x16, x16, #0xec0
+	br	x17
+
+00000000000010d0 <mkdir@plt>:
+	adrp	x16, 12000 <setApiBlacklistExemptions@@Base+0xfe8c>
+	ldr	x17, [x16, #3784]
+	add	x16, x16, #0xec8
+	br	x17
+
+00000000000010e0 <read@plt>:
+	adrp	x16, 12000 <setApiBlacklistExemptions@@Base+0xfe8c>
+	ldr	x17, [x16, #3792]
+	add	x16, x16, #0xed0
+	br	x17
+
+00000000000010f0 <setApiBlacklistExemptions@plt>:
+	adrp	x16, 12000 <setApiBlacklistExemptions@@Base+0xfe8c>
+	ldr	x17, [x16, #3800]
+	add	x16, x16, #0xed8
+	br	x17
+
+0000000000001100 <strtoul@plt>:
+	adrp	x16, 12000 <setApiBlacklistExemptions@@Base+0xfe8c>
 	ldr	x17, [x16, #3808]
 	add	x16, x16, #0xee0
 	br	x17
 
-0000000000000dd0 <munmap@plt>:
-	adrp	x16, 12000 <get_jni_env+0x103e8>
+0000000000001110 <fstat@plt>:
+	adrp	x16, 12000 <setApiBlacklistExemptions@@Base+0xfe8c>
 	ldr	x17, [x16, #3816]
 	add	x16, x16, #0xee8
 	br	x17
 
-0000000000000de0 <fgets@plt>:
-	adrp	x16, 12000 <get_jni_env+0x103e8>
+0000000000001120 <chmod@plt>:
+	adrp	x16, 12000 <setApiBlacklistExemptions@@Base+0xfe8c>
 	ldr	x17, [x16, #3824]
 	add	x16, x16, #0xef0
 	br	x17
 
-0000000000000df0 <getc@plt>:
-	adrp	x16, 12000 <get_jni_env+0x103e8>
+0000000000001130 <setsid@plt>:
+	adrp	x16, 12000 <setApiBlacklistExemptions@@Base+0xfe8c>
 	ldr	x17, [x16, #3832]
 	add	x16, x16, #0xef8
 	br	x17
 
-0000000000000e00 <__cxa_finalize@plt>:
-	adrp	x16, 12000 <get_jni_env+0x103e8>
+0000000000001140 <get_file_size@plt>:
+	adrp	x16, 12000 <setApiBlacklistExemptions@@Base+0xfe8c>
 	ldr	x17, [x16, #3840]
 	add	x16, x16, #0xf00
 	br	x17
 
-0000000000000e10 <getuid@plt>:
-	adrp	x16, 12000 <get_jni_env+0x103e8>
+0000000000001150 <access@plt>:
+	adrp	x16, 12000 <setApiBlacklistExemptions@@Base+0xfe8c>
 	ldr	x17, [x16, #3848]
 	add	x16, x16, #0xf08
 	br	x17
 
-0000000000000e20 <malloc@plt>:
-	adrp	x16, 12000 <get_jni_env+0x103e8>
+0000000000001160 <fclose@plt>:
+	adrp	x16, 12000 <setApiBlacklistExemptions@@Base+0xfe8c>
 	ldr	x17, [x16, #3856]
 	add	x16, x16, #0xf10
 	br	x17
 
-0000000000000e30 <strtoul@plt>:
-	adrp	x16, 12000 <get_jni_env+0x103e8>
+0000000000001170 <fputc@plt>:
+	adrp	x16, 12000 <setApiBlacklistExemptions@@Base+0xfe8c>
 	ldr	x17, [x16, #3864]
 	add	x16, x16, #0xf18
 	br	x17
 
-0000000000000e40 <__android_log_print@plt>:
-	adrp	x16, 12000 <get_jni_env+0x103e8>
+0000000000001180 <__stack_chk_fail@plt>:
+	adrp	x16, 12000 <setApiBlacklistExemptions@@Base+0xfe8c>
 	ldr	x17, [x16, #3872]
 	add	x16, x16, #0xf20
 	br	x17
 
-0000000000000e50 <mmap@plt>:
-	adrp	x16, 12000 <get_jni_env+0x103e8>
+0000000000001190 <fgets@plt>:
+	adrp	x16, 12000 <setApiBlacklistExemptions@@Base+0xfe8c>
 	ldr	x17, [x16, #3880]
 	add	x16, x16, #0xf28
 	br	x17
 
-0000000000000e60 <__stack_chk_fail@plt>:
-	adrp	x16, 12000 <get_jni_env+0x103e8>
+00000000000011a0 <getc@plt>:
+	adrp	x16, 12000 <setApiBlacklistExemptions@@Base+0xfe8c>
 	ldr	x17, [x16, #3888]
 	add	x16, x16, #0xf30
 	br	x17
 
-0000000000000e70 <chmod@plt>:
-	adrp	x16, 12000 <get_jni_env+0x103e8>
+00000000000011b0 <copyfile@plt>:
+	adrp	x16, 12000 <setApiBlacklistExemptions@@Base+0xfe8c>
 	ldr	x17, [x16, #3896]
 	add	x16, x16, #0xf38
 	br	x17
 
-0000000000000e80 <fstat@plt>:
-	adrp	x16, 12000 <get_jni_env+0x103e8>
+00000000000011c0 <get_module_base@plt>:
+	adrp	x16, 12000 <setApiBlacklistExemptions@@Base+0xfe8c>
 	ldr	x17, [x16, #3904]
 	add	x16, x16, #0xf40
 	br	x17
 
-0000000000000e90 <umask@plt>:
-	adrp	x16, 12000 <get_jni_env+0x103e8>
+00000000000011d0 <strncpy@plt>:
+	adrp	x16, 12000 <setApiBlacklistExemptions@@Base+0xfe8c>
 	ldr	x17, [x16, #3912]
 	add	x16, x16, #0xf48
 	br	x17
 
-0000000000000ea0 <strstr@plt>:
-	adrp	x16, 12000 <get_jni_env+0x103e8>
+00000000000011e0 <dlsym@plt>:
+	adrp	x16, 12000 <setApiBlacklistExemptions@@Base+0xfe8c>
 	ldr	x17, [x16, #3920]
 	add	x16, x16, #0xf50
 	br	x17
 
-0000000000000eb0 <read@plt>:
-	adrp	x16, 12000 <get_jni_env+0x103e8>
+00000000000011f0 <__android_log_print@plt>:
+	adrp	x16, 12000 <setApiBlacklistExemptions@@Base+0xfe8c>
 	ldr	x17, [x16, #3928]
 	add	x16, x16, #0xf58
 	br	x17
 
-0000000000000ec0 <strncpy@plt>:
-	adrp	x16, 12000 <get_jni_env+0x103e8>
+0000000000001200 <strcmp@plt>:
+	adrp	x16, 12000 <setApiBlacklistExemptions@@Base+0xfe8c>
 	ldr	x17, [x16, #3936]
 	add	x16, x16, #0xf60
 	br	x17
 
-0000000000000ed0 <__cxa_atexit@plt>:
-	adrp	x16, 12000 <get_jni_env+0x103e8>
+0000000000001210 <sprintf@plt>:
+	adrp	x16, 12000 <setApiBlacklistExemptions@@Base+0xfe8c>
 	ldr	x17, [x16, #3944]
 	add	x16, x16, #0xf68
 	br	x17
 
-0000000000000ee0 <strtok@plt>:
-	adrp	x16, 12000 <get_jni_env+0x103e8>
+0000000000001220 <mmap@plt>:
+	adrp	x16, 12000 <setApiBlacklistExemptions@@Base+0xfe8c>
 	ldr	x17, [x16, #3952]
 	add	x16, x16, #0xf70
 	br	x17
 
-0000000000000ef0 <dlsym@plt>:
-	adrp	x16, 12000 <get_jni_env+0x103e8>
+0000000000001230 <get_symbol_offset@plt>:
+	adrp	x16, 12000 <setApiBlacklistExemptions@@Base+0xfe8c>
 	ldr	x17, [x16, #3960]
 	add	x16, x16, #0xf78
 	br	x17
 
-0000000000000f00 <fopen@plt>:
-	adrp	x16, 12000 <get_jni_env+0x103e8>
+0000000000001240 <get_sdk_version@plt>:
+	adrp	x16, 12000 <setApiBlacklistExemptions@@Base+0xfe8c>
 	ldr	x17, [x16, #3968]
 	add	x16, x16, #0xf80
 	br	x17
 
-0000000000000f10 <memset@plt>:
-	adrp	x16, 12000 <get_jni_env+0x103e8>
+0000000000001250 <getuid@plt>:
+	adrp	x16, 12000 <setApiBlacklistExemptions@@Base+0xfe8c>
 	ldr	x17, [x16, #3976]
 	add	x16, x16, #0xf88
 	br	x17
 
-0000000000000f20 <fclose@plt>:
-	adrp	x16, 12000 <get_jni_env+0x103e8>
+0000000000001260 <strstr@plt>:
+	adrp	x16, 12000 <setApiBlacklistExemptions@@Base+0xfe8c>
 	ldr	x17, [x16, #3984]
 	add	x16, x16, #0xf90
 	br	x17
 
-0000000000000f30 <strcmp@plt>:
-	adrp	x16, 12000 <get_jni_env+0x103e8>
+0000000000001270 <strtok@plt>:
+	adrp	x16, 12000 <setApiBlacklistExemptions@@Base+0xfe8c>
 	ldr	x17, [x16, #3992]
 	add	x16, x16, #0xf98
 	br	x17
 
-0000000000000f40 <sprintf@plt>:
-	adrp	x16, 12000 <get_jni_env+0x103e8>
+0000000000001280 <close@plt>:
+	adrp	x16, 12000 <setApiBlacklistExemptions@@Base+0xfe8c>
 	ldr	x17, [x16, #4000]
 	add	x16, x16, #0xfa0
 	br	x17
 
-0000000000000f50 <fputc@plt>:
-	adrp	x16, 12000 <get_jni_env+0x103e8>
+0000000000001290 <stat@plt>:
+	adrp	x16, 12000 <setApiBlacklistExemptions@@Base+0xfe8c>
 	ldr	x17, [x16, #4008]
 	add	x16, x16, #0xfa8
 	br	x17
 
-0000000000000f60 <stat@plt>:
-	adrp	x16, 12000 <get_jni_env+0x103e8>
+00000000000012a0 <munmap@plt>:
+	adrp	x16, 12000 <setApiBlacklistExemptions@@Base+0xfe8c>
 	ldr	x17, [x16, #4016]
 	add	x16, x16, #0xfb0
 	br	x17
 
-0000000000000f70 <access@plt>:
-	adrp	x16, 12000 <get_jni_env+0x103e8>
+00000000000012b0 <malloc@plt>:
+	adrp	x16, 12000 <setApiBlacklistExemptions@@Base+0xfe8c>
 	ldr	x17, [x16, #4024]
 	add	x16, x16, #0xfb8
 	br	x17
 
-0000000000000f80 <open@plt>:
-	adrp	x16, 12000 <get_jni_env+0x103e8>
+00000000000012c0 <memset@plt>:
+	adrp	x16, 12000 <setApiBlacklistExemptions@@Base+0xfe8c>
 	ldr	x17, [x16, #4032]
 	add	x16, x16, #0xfc0
 	br	x17
 
-0000000000000f90 <setsid@plt>:
-	adrp	x16, 12000 <get_jni_env+0x103e8>
+00000000000012d0 <fopen@plt>:
+	adrp	x16, 12000 <setApiBlacklistExemptions@@Base+0xfe8c>
 	ldr	x17, [x16, #4040]
 	add	x16, x16, #0xfc8
 	br	x17
 
-0000000000000fa0 <mkdir@plt>:
-	adrp	x16, 12000 <get_jni_env+0x103e8>
+00000000000012e0 <free@plt>:
+	adrp	x16, 12000 <setApiBlacklistExemptions@@Base+0xfe8c>
 	ldr	x17, [x16, #4048]
 	add	x16, x16, #0xfd0
 	br	x17
 
-0000000000000fb0 <close@plt>:
-	adrp	x16, 12000 <get_jni_env+0x103e8>
+00000000000012f0 <__system_property_get@plt>:
+	adrp	x16, 12000 <setApiBlacklistExemptions@@Base+0xfe8c>
 	ldr	x17, [x16, #4056]
 	add	x16, x16, #0xfd8
 	br	x17
 
-0000000000000fc0 <free@plt>:
-	adrp	x16, 12000 <get_jni_env+0x103e8>
+0000000000001300 <get_jni_env@plt>:
+	adrp	x16, 12000 <setApiBlacklistExemptions@@Base+0xfe8c>
 	ldr	x17, [x16, #4064]
 	add	x16, x16, #0xfe0
 	br	x17
+
+0000000000001310 <__cxa_atexit@plt>:
+	adrp	x16, 12000 <setApiBlacklistExemptions@@Base+0xfe8c>
+	ldr	x17, [x16, #4072]
+	add	x16, x16, #0xfe8
+	br	x17
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text {}

```diff
@@ -1,887 +1,1064 @@
 
 
 
 Disassembly of section .text:
 
-0000000000000fd0 <load_dex_in_thread-0x3c>:
-	adrp	x0, 13000 <get_jni_env+0x113e8>
+0000000000001320 <load_dex_in_thread@@Base-0x3c>:
+	adrp	x0, 13000 <setApiBlacklistExemptions@@Base+0x10e8c>
 	add	x0, x0, #0x0
-	b	e00 <__cxa_finalize@plt>
+	b	10c0 <__cxa_finalize@plt>
 	stp	x29, x30, [sp, #-16]!
 	mov	x29, sp
-	cbz	x0, fec <free@plt+0x2c>
+	cbz	x0, 133c <__cxa_atexit@plt+0x2c>
 	blr	x0
 	ldp	x29, x30, [sp], #16
 	ret
 	mov	x1, x0
-	adrp	x2, 13000 <get_jni_env+0x113e8>
-	adrp	x0, 0 <pthread_create@plt-0xdc0>
+	adrp	x2, 13000 <setApiBlacklistExemptions@@Base+0x10e8c>
+	adrp	x0, 1000 <atoi@plt-0x80>
 	add	x2, x2, #0x0
-	add	x0, x0, #0xfdc
-	b	ed0 <__cxa_atexit@plt>
+	add	x0, x0, #0x32c
+	b	1310 <__cxa_atexit@plt>
 
-000000000000100c <load_dex_in_thread>:
+000000000000135c <load_dex_in_thread@@Base>:
 	sub	sp, sp, #0x60
-	adrp	x2, 1000 <free@plt+0x40>
-	add	x2, x2, #0xd60
-	stp	x21, x22, [sp, #16]
-	adrp	x21, 12000 <get_jni_env+0x103e8>
-	stp	x19, x20, [sp]
-	stp	x23, x24, [sp, #32]
-	ldr	x3, [x21, #4080]
-	adrp	x19, 1000 <free@plt+0x40>
-	stp	x25, x30, [sp, #48]
-	add	x19, x19, #0xd50
-	mov	x20, x0
-	ldr	x3, [x3]
-	mov	x1, x19
-	mov	w0, #0x4                   	// #4
-	str	x3, [sp, #88]
-	bl	e40 <__android_log_print@plt>
-	ldr	x24, [x20]
-	add	x1, sp, #0x60
-	mov	x2, #0x0                   	// #0
-	mov	x0, x24
-	str	x2, [x1, #-16]!
-	ldr	x3, [x24]
-	ldr	x3, [x3, #32]
-	blr	x3
-	ldr	x3, [sp, #80]
-	cbz	x3, 1348 <load_dex_in_thread+0x33c>
-	adrp	x2, 1000 <free@plt+0x40>
-	mov	x1, x19
-	add	x2, x2, #0xd80
-	mov	w0, #0x4                   	// #4
-	add	x23, x20, #0x210
-	bl	e40 <__android_log_print@plt>
-	ldr	x2, [sp, #80]
-	adrp	x1, 1000 <free@plt+0x40>
-	add	x1, x1, #0xd98
-	mov	x0, x2
-	ldr	x2, [x2]
-	ldr	x2, [x2, #48]
-	blr	x2
-	mov	x22, x0
-	ldr	x0, [sp, #80]
-	adrp	x3, 1000 <free@plt+0x40>
-	adrp	x2, 1000 <free@plt+0x40>
-	mov	x1, x22
-	add	x3, x3, #0xdc8
-	add	x2, x2, #0xdb0
-	ldr	x4, [x0]
-	ldr	x4, [x4, #904]
-	blr	x4
+	str	x25, [sp, #16]
+	stp	x24, x23, [sp, #32]
+	stp	x22, x21, [sp, #48]
+	stp	x20, x19, [sp, #64]
+	stp	x29, x30, [sp, #80]
+	add	x29, sp, #0x50
+	mrs	x25, tpidr_el0
+	ldr	x8, [x25, #40]
+	adrp	x1, 2000 <get_symbol_offset@@Base+0x2d4>
+	adrp	x2, 2000 <get_symbol_offset@@Base+0x2d4>
+	mov	x19, x0
+	add	x1, x1, #0x348
+	add	x2, x2, #0x352
+	orr	w0, wzr, #0x4
+	str	x8, [sp, #8]
+	bl	11f0 <__android_log_print@plt>
+	ldr	x20, [x19]
+	str	xzr, [sp]
+	mov	x1, sp
+	mov	x2, xzr
+	ldr	x8, [x20]
+	mov	x0, x20
+	ldr	x8, [x8, #32]
+	blr	x8
+	ldr	x3, [sp]
+	cbz	x3, 1610 <load_dex_in_thread@@Base+0x2b4>
+	adrp	x1, 2000 <get_symbol_offset@@Base+0x2d4>
+	adrp	x2, 2000 <get_symbol_offset@@Base+0x2d4>
+	add	x1, x1, #0x348
+	add	x2, x2, #0x36e
+	orr	w0, wzr, #0x4
+	bl	11f0 <__android_log_print@plt>
+	bl	1240 <get_sdk_version@plt>
+	cmp	w0, #0x1e
+	b.lt	140c <load_dex_in_thread@@Base+0xb0>  // b.tstop
+	adrp	x1, 2000 <get_symbol_offset@@Base+0x2d4>
+	adrp	x2, 2000 <get_symbol_offset@@Base+0x2d4>
+	add	x1, x1, #0x348
+	add	x2, x2, #0x381
+	orr	w0, wzr, #0x4
+	bl	11f0 <__android_log_print@plt>
+	ldr	x0, [sp]
+	bl	10f0 <setApiBlacklistExemptions@plt>
+	ldr	x0, [sp]
+	adrp	x1, 2000 <get_symbol_offset@@Base+0x2d4>
+	add	x1, x1, #0x3a0
+	ldr	x8, [x0]
+	ldr	x8, [x8, #48]
+	blr	x8
+	ldr	x8, [sp]
+	mov	x21, x0
+	adrp	x2, 2000 <get_symbol_offset@@Base+0x2d4>
+	adrp	x3, 2000 <get_symbol_offset@@Base+0x2d4>
+	ldr	x9, [x8]
+	add	x2, x2, #0x3b6
+	add	x3, x3, #0x3cb
+	mov	x0, x8
+	ldr	x9, [x9, #904]
+	mov	x1, x21
+	blr	x9
+	ldr	x8, [sp]
 	mov	x2, x0
-	ldr	x3, [sp, #80]
-	mov	x1, x22
-	mov	x0, x3
-	ldr	x3, [x3]
-	ldr	x3, [x3, #912]
-	blr	x3
-	str	x0, [sp, #72]
-	ldr	x2, [sp, #80]
-	add	x1, x20, #0x8
-	mov	x0, x2
-	ldr	x2, [x2]
-	ldr	x2, [x2, #1336]
-	blr	x2
-	mov	x25, x0
-	ldr	x2, [sp, #80]
-	add	x1, x20, #0x10c
-	mov	x0, x2
-	ldr	x2, [x2]
-	ldr	x2, [x2, #1336]
-	blr	x2
-	str	x0, [sp, #64]
-	ldr	x2, [sp, #80]
-	adrp	x1, 1000 <free@plt+0x40>
-	add	x1, x1, #0xde8
-	mov	x0, x2
-	ldr	x2, [x2]
-	ldr	x2, [x2, #48]
-	blr	x2
+	mov	x1, x21
+	ldr	x9, [x8]
+	mov	x0, x8
+	ldr	x9, [x9, #912]
+	blr	x9
+	mov	x21, x0
+	ldr	x0, [sp]
+	add	x1, x19, #0x8
+	ldr	x8, [x0]
+	ldr	x8, [x8, #1336]
+	blr	x8
 	mov	x22, x0
-	ldr	x0, [sp, #80]
-	adrp	x2, 1000 <free@plt+0x40>
-	adrp	x3, 1000 <free@plt+0x40>
-	mov	x1, x22
-	add	x2, x2, #0xe08
-	add	x3, x3, #0xe10
-	ldr	x7, [x0]
-	ldr	x5, [x7, #264]
-	blr	x5
+	ldr	x0, [sp]
+	add	x1, x19, #0x10c
+	ldr	x8, [x0]
+	ldr	x8, [x8, #1336]
+	blr	x8
+	ldr	x8, [sp]
+	adrp	x1, 2000 <get_symbol_offset@@Base+0x2d4>
+	mov	x23, x0
+	add	x1, x1, #0x3e5
+	ldr	x9, [x8]
+	mov	x0, x8
+	ldr	x9, [x9, #48]
+	blr	x9
+	ldr	x8, [sp]
+	mov	x24, x0
+	adrp	x2, 2000 <get_symbol_offset@@Base+0x2d4>
+	adrp	x3, 2000 <get_symbol_offset@@Base+0x2d4>
+	ldr	x9, [x8]
+	add	x2, x2, #0x402
+	add	x3, x3, #0x409
+	mov	x0, x8
+	ldr	x9, [x9, #264]
+	mov	x1, x24
+	blr	x9
+	ldr	x8, [sp]
 	mov	x2, x0
-	ldr	x0, [sp, #80]
-	mov	x5, #0x0                   	// #0
-	ldr	x6, [sp, #72]
-	mov	x1, x22
-	ldr	x4, [sp, #64]
-	mov	x3, x25
+	mov	x1, x24
+	mov	x3, x22
+	ldr	x9, [x8]
+	mov	x0, x8
+	mov	x4, x23
+	mov	x5, xzr
+	ldr	x9, [x9, #224]
+	mov	x6, x21
+	blr	x9
+	adrp	x23, 2000 <get_symbol_offset@@Base+0x2d4>
+	mov	x22, x0
+	add	x23, x23, #0x348
+	adrp	x2, 2000 <get_symbol_offset@@Base+0x2d4>
+	add	x2, x2, #0x45a
+	orr	w0, wzr, #0x4
+	mov	x1, x23
+	mov	x3, x22
+	bl	11f0 <__android_log_print@plt>
+	ldr	x0, [sp]
+	adrp	x2, 2000 <get_symbol_offset@@Base+0x2d4>
+	adrp	x3, 2000 <get_symbol_offset@@Base+0x2d4>
+	add	x2, x2, #0x470
 	ldr	x8, [x0]
-	ldr	x7, [x8, #224]
-	blr	x7
+	add	x3, x3, #0x47a
+	mov	x1, x24
+	ldr	x8, [x8, #264]
+	blr	x8
+	mov	x24, x0
+	ldr	x0, [sp]
+	add	x21, x19, #0x210
+	mov	x1, x21
+	ldr	x8, [x0]
+	ldr	x8, [x8, #1336]
+	blr	x8
+	ldr	x8, [sp]
 	mov	x3, x0
-	adrp	x2, 1000 <free@plt+0x40>
-	mov	x25, x0
-	mov	x1, x19
-	add	x2, x2, #0xe68
-	mov	w0, #0x4                   	// #4
-	bl	e40 <__android_log_print@plt>
-	ldr	x0, [sp, #80]
-	adrp	x2, 1000 <free@plt+0x40>
-	adrp	x3, 1000 <free@plt+0x40>
-	add	x2, x2, #0xe80
 	mov	x1, x22
-	add	x3, x3, #0xe90
-	ldr	x4, [x0]
-	ldr	x4, [x4, #264]
-	blr	x4
-	str	x0, [sp, #64]
-	ldr	x3, [sp, #80]
-	mov	x1, x23
-	mov	x0, x3
-	ldr	x3, [x3]
-	ldr	x3, [x3, #1336]
-	blr	x3
-	mov	x3, x0
-	ldr	x4, [sp, #80]
-	mov	x1, x25
-	ldr	x2, [sp, #64]
-	mov	x0, x4
-	ldr	x4, [x4]
-	ldr	x4, [x4, #272]
-	blr	x4
+	mov	x2, x24
+	ldr	x9, [x8]
+	mov	x0, x8
+	ldr	x9, [x9, #272]
+	blr	x9
 	mov	x22, x0
-	adrp	x2, 1000 <free@plt+0x40>
-	mov	x1, x19
-	add	x2, x2, #0xeb8
-	mov	w0, #0x4                   	// #4
-	mov	x3, x23
+	adrp	x2, 2000 <get_symbol_offset@@Base+0x2d4>
+	add	x2, x2, #0x4a0
+	orr	w0, wzr, #0x4
+	mov	x1, x23
+	mov	x3, x21
 	mov	x4, x22
-	bl	e40 <__android_log_print@plt>
-	ldr	x2, [sp, #80]
-	mov	x0, x2
-	ldr	x1, [x2]
-	ldr	x1, [x1, #120]
-	blr	x1
-	cbz	x0, 12bc <load_dex_in_thread+0x2b0>
-	ldr	x1, [sp, #80]
-	mov	x0, x1
-	ldr	x1, [x1]
-	ldr	x1, [x1, #128]
-	blr	x1
-	ldr	x1, [sp, #80]
-	mov	x0, x1
-	ldr	x1, [x1]
-	ldr	x1, [x1, #136]
-	blr	x1
-	adrp	x2, 1000 <free@plt+0x40>
-	mov	x1, x19
-	add	x2, x2, #0xec8
-	mov	x3, x23
-	mov	w0, #0x6                   	// #6
-	bl	e40 <__android_log_print@plt>
-	ldr	x21, [x21, #4080]
-	mov	x0, #0x0                   	// #0
-	ldr	x2, [sp, #88]
-	ldr	x1, [x21]
-	cmp	x2, x1
-	b.ne	1360 <load_dex_in_thread+0x354>  // b.any
-	ldp	x19, x20, [sp]
-	ldp	x21, x22, [sp, #16]
-	ldp	x23, x24, [sp, #32]
-	ldp	x25, x30, [sp, #48]
-	add	sp, sp, #0x60
-	ret
-	ldr	x4, [sp, #80]
-	add	x2, x20, #0x314
-	add	x3, x20, #0x418
+	bl	11f0 <__android_log_print@plt>
+	ldr	x0, [sp]
+	ldr	x8, [x0]
+	ldr	x8, [x8, #120]
+	blr	x8
+	ldr	x8, [sp]
+	ldr	x9, [x8]
+	cbz	x0, 1628 <load_dex_in_thread@@Base+0x2cc>
+	ldr	x9, [x9, #128]
+	mov	x0, x8
+	blr	x9
+	ldr	x0, [sp]
+	ldr	x8, [x0]
+	ldr	x8, [x8, #136]
+	blr	x8
+	adrp	x1, 2000 <get_symbol_offset@@Base+0x2d4>
+	adrp	x2, 2000 <get_symbol_offset@@Base+0x2d4>
+	add	x1, x1, #0x348
+	add	x2, x2, #0x4ad
+	orr	w0, wzr, #0x6
+	mov	x3, x21
+	bl	11f0 <__android_log_print@plt>
+	b	16a8 <load_dex_in_thread@@Base+0x34c>
+	adrp	x1, 2000 <get_symbol_offset@@Base+0x2d4>
+	adrp	x2, 2000 <get_symbol_offset@@Base+0x2d4>
+	add	x1, x1, #0x348
+	add	x2, x2, #0x35f
+	orr	w0, wzr, #0x6
+	b	16a4 <load_dex_in_thread@@Base+0x348>
+	ldr	x9, [x9, #904]
+	add	x2, x19, #0x314
+	add	x3, x19, #0x418
+	mov	x0, x8
 	mov	x1, x22
-	mov	x0, x4
-	ldr	x4, [x4]
-	ldr	x4, [x4, #904]
-	blr	x4
-	str	x0, [sp, #64]
-	ldr	x3, [sp, #80]
-	add	x1, x20, #0x51c
-	mov	x0, x3
-	ldr	x3, [x3]
-	ldr	x3, [x3, #1336]
-	blr	x3
+	blr	x9
+	mov	x21, x0
+	ldr	x0, [sp]
+	add	x1, x19, #0x51c
+	ldr	x8, [x0]
+	ldr	x8, [x8, #1336]
+	blr	x8
+	ldr	x8, [sp]
 	mov	x3, x0
-	ldr	x4, [sp, #80]
 	mov	x1, x22
-	ldr	x2, [sp, #64]
-	mov	x0, x4
-	ldr	x4, [x4]
-	ldr	x4, [x4, #1128]
-	blr	x4
-	ldr	x1, [x24]
-	mov	x0, x24
-	ldr	x1, [x1, #40]
-	blr	x1
+	mov	x2, x21
+	ldr	x9, [x8]
+	mov	x0, x8
+	ldr	x9, [x9, #1128]
+	blr	x9
+	ldr	x8, [x20]
 	mov	x0, x20
-	bl	fc0 <free@plt>
-	adrp	x2, 1000 <free@plt+0x40>
-	mov	x1, x19
-	add	x2, x2, #0xee0
-	mov	w0, #0x4                   	// #4
-	bl	e40 <__android_log_print@plt>
-	b	128c <load_dex_in_thread+0x280>
-	adrp	x2, 1000 <free@plt+0x40>
-	mov	x1, x19
-	add	x2, x2, #0xd70
-	mov	w0, #0x6                   	// #6
-	bl	e40 <__android_log_print@plt>
-	b	128c <load_dex_in_thread+0x280>
-	bl	e60 <__stack_chk_fail@plt>
+	ldr	x8, [x8, #40]
+	blr	x8
+	mov	x0, x19
+	bl	12e0 <free@plt>
+	adrp	x1, 2000 <get_symbol_offset@@Base+0x2d4>
+	adrp	x2, 2000 <get_symbol_offset@@Base+0x2d4>
+	add	x1, x1, #0x348
+	add	x2, x2, #0x4c2
+	orr	w0, wzr, #0x4
+	bl	11f0 <__android_log_print@plt>
+	ldr	x8, [x25, #40]
+	ldr	x9, [sp, #8]
+	cmp	x8, x9
+	b.ne	16d8 <load_dex_in_thread@@Base+0x37c>  // b.any
+	ldp	x29, x30, [sp, #80]
+	ldp	x20, x19, [sp, #64]
+	ldp	x22, x21, [sp, #48]
+	ldp	x24, x23, [sp, #32]
+	ldr	x25, [sp, #16]
+	mov	x0, xzr
+	add	sp, sp, #0x60
+	ret
+	bl	1180 <__stack_chk_fail@plt>
 
-0000000000001364 <load_dex>:
-	sub	sp, sp, #0x340
-	sub	sp, sp, #0x60
-	stp	x21, x22, [sp, #16]
-	adrp	x22, 12000 <get_jni_env+0x103e8>
-	str	x30, [sp, #80]
-	stp	x23, x24, [sp, #32]
-	stp	x25, x26, [sp, #48]
-	ldr	x8, [x22, #4080]
-	mov	x23, x1
-	stp	x19, x20, [sp]
-	stp	x27, x28, [sp, #64]
-	mov	x25, x3
-	mov	x24, x5
-	ldr	x8, [x8]
-	mov	x5, x2
-	mov	x26, x2
-	adrp	x21, 1000 <free@plt+0x40>
-	adrp	x2, 1000 <free@plt+0x40>
-	mov	x3, x0
-	mov	x6, x25
-	mov	x7, x24
-	add	x1, x21, #0xd50
-	add	x2, x2, #0xef0
-	str	x4, [sp, #104]
-	mov	x27, x0
-	mov	x4, x23
-	mov	w0, #0x4                   	// #4
-	str	x8, [sp, #920]
-	add	x20, sp, #0x80
-	bl	e40 <__android_log_print@plt>
-	mov	x2, #0x104                 	// #260
-	mov	w1, #0x0                   	// #0
-	mov	x0, x20
-	bl	f10 <memset@plt>
-	mov	x0, x20
-	mov	x1, x23
-	mov	x2, #0x104                 	// #260
-	bl	ec0 <strncpy@plt>
-	mov	x8, x20
-	ldrb	w9, [x8]
-	cbz	w9, 1628 <load_dex+0x2c4>
-	adds	x8, x8, #0x1
-	b.ne	1400 <load_dex+0x9c>  // b.any
-	mov	x8, #0xffffffffffffffff    	// #-1
-	ldrb	w0, [x8]
-	cmp	w0, #0x2f
-	b.ne	1430 <load_dex+0xcc>  // b.any
-	b	1444 <load_dex+0xe0>
-	ldrb	w9, [x8]
-	cmp	w9, #0x2f
-	b.eq	1444 <load_dex+0xe0>  // b.none
-	subs	x8, x8, #0x1
-	b.ne	1424 <load_dex+0xc0>  // b.any
-	mov	x0, #0x0                   	// #0
-	strb	w0, [x0]
-	brk	#0x3e8
-	mov	x19, x8
-	add	x28, sp, #0x188
-	mov	x2, #0x104                 	// #260
-	mov	w1, #0x0                   	// #0
-	mov	x0, x28
-	strb	wzr, [x19], #1
-	bl	f10 <memset@plt>
-	mov	x1, x19
-	mov	x2, #0x104                 	// #260
-	mov	x0, x28
-	bl	ec0 <strncpy@plt>
-	bl	e10 <getuid@plt>
+00000000000016dc <load_dex@@Base>:
+	str	x28, [sp, #-96]!
+	stp	x26, x25, [sp, #16]
+	stp	x24, x23, [sp, #32]
+	stp	x22, x21, [sp, #48]
+	stp	x20, x19, [sp, #64]
+	stp	x29, x30, [sp, #80]
+	add	x29, sp, #0x50
+	sub	sp, sp, #0x330
+	mrs	x26, tpidr_el0
+	ldr	x8, [x26, #40]
+	mov	x19, x5
+	mov	x21, x3
+	mov	x22, x2
+	mov	x24, x1
+	mov	x23, x0
+	adrp	x1, 2000 <get_symbol_offset@@Base+0x2d4>
+	adrp	x2, 2000 <get_symbol_offset@@Base+0x2d4>
+	mov	x20, x4
+	add	x1, x1, #0x348
+	add	x2, x2, #0x4ce
+	orr	w0, wzr, #0x4
+	mov	x3, x23
+	mov	x4, x24
+	mov	x5, x22
+	mov	x6, x21
+	mov	x7, x19
+	stur	x8, [x29, #-88]
+	bl	11f0 <__android_log_print@plt>
+	add	x0, sp, #0x224
+	mov	w2, #0x104                 	// #260
+	mov	w1, wzr
+	add	x25, sp, #0x224
+	bl	12c0 <memset@plt>
+	add	x0, sp, #0x224
+	mov	w2, #0x104                 	// #260
+	mov	x1, x24
+	bl	11d0 <strncpy@plt>
+	ldrb	w8, [x25], #1
+	cbnz	w8, 1770 <load_dex@@Base+0x94>
+	ldurb	w8, [x25, #-2]
+	sub	x25, x25, #0x1
+	cmp	w8, #0x2f
+	b.ne	1778 <load_dex@@Base+0x9c>  // b.any
+	add	x0, sp, #0x120
+	mov	w2, #0x104                 	// #260
+	mov	w1, wzr
+	sturb	wzr, [x25, #-1]
+	bl	12c0 <memset@plt>
+	add	x0, sp, #0x120
+	mov	w2, #0x104                 	// #260
+	mov	x1, x25
+	bl	11d0 <strncpy@plt>
+	bl	1250 <getuid@plt>
+	adrp	x1, 2000 <get_symbol_offset@@Base+0x2d4>
 	mov	w3, w0
-	adrp	x1, 1000 <free@plt+0x40>
-	mov	x2, x20
-	add	x1, x1, #0xf18
-	mov	x0, x20
-	bl	f40 <sprintf@plt>
-	adrp	x2, 1000 <free@plt+0x40>
-	add	x1, x21, #0xd50
-	add	x2, x2, #0xf20
-	mov	x3, x20
-	mov	w0, #0x4                   	// #4
-	bl	e40 <__android_log_print@plt>
-	mov	x0, x20
-	mov	w1, #0x0                   	// #0
-	bl	f70 <access@plt>
+	add	x1, x1, #0x4f4
+	add	x0, sp, #0x224
+	add	x2, sp, #0x224
+	bl	1210 <sprintf@plt>
+	adrp	x1, 2000 <get_symbol_offset@@Base+0x2d4>
+	adrp	x2, 2000 <get_symbol_offset@@Base+0x2d4>
+	add	x1, x1, #0x348
+	add	x2, x2, #0x4fa
+	orr	w0, wzr, #0x4
+	add	x3, sp, #0x224
+	bl	11f0 <__android_log_print@plt>
+	add	x0, sp, #0x224
+	mov	w1, wzr
+	bl	1150 <access@plt>
 	cmn	w0, #0x1
-	b.eq	166c <load_dex+0x308>  // b.none
-	add	x19, sp, #0x290
-	mov	w1, #0x0                   	// #0
-	mov	x2, #0x104                 	// #260
-	mov	x0, x19
-	bl	f10 <memset@plt>
-	adrp	x1, 1000 <free@plt+0x40>
-	mov	x3, x28
-	add	x1, x1, #0xf38
-	mov	x2, x20
-	mov	x0, x19
-	bl	f40 <sprintf@plt>
-	mov	x0, x23
-	bl	16c4 <get_file_size>
-	sxtw	x28, w0
-	cbnz	x28, 1634 <load_dex+0x2d0>
-	bl	1c18 <get_jni_env>
-	add	x21, x21, #0xd50
-	adrp	x2, 1000 <free@plt+0x40>
-	mov	x19, x0
-	mov	x3, x0
-	mov	x1, x21
-	add	x2, x2, #0xf40
-	mov	w0, #0x4                   	// #4
-	add	x28, sp, #0x70
-	bl	e40 <__android_log_print@plt>
-	ldr	x2, [x19]
-	mov	x0, x19
-	mov	x1, x28
-	ldr	x2, [x2, #1752]
-	blr	x2
-	mov	w23, w0
-	cbnz	w0, 167c <load_dex+0x318>
-	ldr	x3, [x28]
-	adrp	x2, 1000 <free@plt+0x40>
+	b.ne	1804 <load_dex@@Base+0x128>  // b.any
+	add	x0, sp, #0x224
+	orr	w1, wzr, #0x1ff
+	bl	10d0 <mkdir@plt>
+	add	x0, sp, #0x1c
+	mov	w2, #0x104                 	// #260
+	mov	w1, wzr
+	bl	12c0 <memset@plt>
+	adrp	x1, 2000 <get_symbol_offset@@Base+0x2d4>
+	add	x1, x1, #0x50b
+	add	x0, sp, #0x1c
+	add	x2, sp, #0x224
+	add	x3, sp, #0x120
+	bl	1210 <sprintf@plt>
+	mov	x0, x24
+	bl	1140 <get_file_size@plt>
+	mov	w25, w0
+	cbz	w25, 1870 <load_dex@@Base+0x194>
+	add	x0, sp, #0x1c
+	bl	1140 <get_file_size@plt>
+	cmp	w25, w0
+	b.eq	1870 <load_dex@@Base+0x194>  // b.none
+	add	x0, sp, #0x224
+	orr	w1, wzr, #0x1ff
+	bl	1120 <chmod@plt>
+	add	x1, sp, #0x1c
+	mov	x0, x24
+	bl	11b0 <copyfile@plt>
+	add	x0, sp, #0x1c
+	orr	w1, wzr, #0x1ff
+	bl	1120 <chmod@plt>
+	bl	1300 <get_jni_env@plt>
+	mov	x24, x0
+	adrp	x1, 2000 <get_symbol_offset@@Base+0x2d4>
+	adrp	x2, 2000 <get_symbol_offset@@Base+0x2d4>
+	add	x1, x1, #0x348
+	add	x2, x2, #0x511
+	orr	w0, wzr, #0x4
+	mov	x3, x24
+	bl	11f0 <__android_log_print@plt>
+	ldr	x8, [x24]
+	add	x1, sp, #0x10
+	mov	x0, x24
+	ldr	x8, [x8, #1752]
+	blr	x8
+	mov	w8, w0
+	cbz	w8, 18d4 <load_dex@@Base+0x1f8>
+	adrp	x1, 2000 <get_symbol_offset@@Base+0x2d4>
+	adrp	x2, 2000 <get_symbol_offset@@Base+0x2d4>
+	add	x1, x1, #0x348
+	add	x2, x2, #0x51d
+	orr	w0, wzr, #0x6
+	mov	w3, w8
+	bl	11f0 <__android_log_print@plt>
+	mov	w0, #0xffffffff            	// #-1
+	b	1994 <load_dex@@Base+0x2b8>
+	ldr	x3, [sp, #16]
+	adrp	x24, 2000 <get_symbol_offset@@Base+0x2d4>
+	add	x24, x24, #0x348
+	adrp	x2, 2000 <get_symbol_offset@@Base+0x2d4>
+	add	x2, x2, #0x530
+	orr	w0, wzr, #0x4
+	mov	x1, x24
+	bl	11f0 <__android_log_print@plt>
+	mov	w0, #0x620                 	// #1568
+	bl	12b0 <malloc@plt>
+	ldr	x8, [sp, #16]
+	mov	x25, x0
+	mov	w2, #0x104                 	// #260
+	mov	x1, x23
+	str	x8, [x0], #8
+	bl	11d0 <strncpy@plt>
+	add	x0, x25, #0x10c
+	add	x1, sp, #0x224
+	mov	w2, #0x104                 	// #260
+	bl	11d0 <strncpy@plt>
+	add	x0, x25, #0x210
+	mov	w2, #0x104                 	// #260
+	mov	x1, x22
+	bl	11d0 <strncpy@plt>
+	add	x0, x25, #0x314
+	mov	w2, #0x104                 	// #260
 	mov	x1, x21
-	add	x2, x2, #0xf68
-	mov	w0, #0x4                   	// #4
-	bl	e40 <__android_log_print@plt>
-	mov	x0, #0x620                 	// #1568
-	bl	e20 <malloc@plt>
-	mov	x19, x0
-	ldr	x3, [x28]
-	mov	x1, x27
-	str	x3, [x0], #8
-	mov	x2, #0x104                 	// #260
-	bl	ec0 <strncpy@plt>
+	bl	11d0 <strncpy@plt>
+	add	x0, x25, #0x418
+	mov	w2, #0x104                 	// #260
 	mov	x1, x20
-	mov	x2, #0x104                 	// #260
-	add	x0, x19, #0x10c
-	bl	ec0 <strncpy@plt>
-	mov	x1, x26
-	mov	x2, #0x104                 	// #260
-	add	x0, x19, #0x210
-	bl	ec0 <strncpy@plt>
-	mov	x1, x25
-	mov	x2, #0x104                 	// #260
-	add	x0, x19, #0x314
-	bl	ec0 <strncpy@plt>
-	ldr	x1, [sp, #104]
-	mov	x2, #0x104                 	// #260
-	add	x0, x19, #0x418
-	bl	ec0 <strncpy@plt>
+	bl	11d0 <strncpy@plt>
+	add	x0, x25, #0x51c
+	mov	w2, #0x104                 	// #260
+	mov	x1, x19
+	bl	11d0 <strncpy@plt>
+	adrp	x2, 2000 <get_symbol_offset@@Base+0x2d4>
+	add	x2, x2, #0x53b
+	orr	w0, wzr, #0x4
 	mov	x1, x24
-	mov	x2, #0x104                 	// #260
-	add	x0, x19, #0x51c
-	bl	ec0 <strncpy@plt>
-	adrp	x2, 1000 <free@plt+0x40>
-	mov	x1, x21
-	add	x2, x2, #0xf78
-	mov	w0, #0x4                   	// #4
-	bl	e40 <__android_log_print@plt>
-	adrp	x2, 12000 <get_jni_env+0x103e8>
-	add	x0, sp, #0x78
-	mov	x1, #0x0                   	// #0
-	mov	x3, x19
+	bl	11f0 <__android_log_print@plt>
+	adrp	x2, 12000 <setApiBlacklistExemptions@@Base+0xfe8c>
 	ldr	x2, [x2, #4088]
-	bl	dc0 <pthread_create@plt>
-	mov	w0, w23
-	ldr	x22, [x22, #4080]
-	ldr	x2, [sp, #920]
-	ldr	x1, [x22]
-	cmp	x2, x1
-	b.ne	169c <load_dex+0x338>  // b.any
-	ldp	x19, x20, [sp]
-	ldp	x21, x22, [sp, #16]
-	ldp	x23, x24, [sp, #32]
-	ldp	x25, x26, [sp, #48]
-	ldp	x27, x28, [sp, #64]
-	ldr	x30, [sp, #80]
-	add	sp, sp, #0x60
-	add	sp, sp, #0x340
+	add	x0, sp, #0x8
+	mov	x1, xzr
+	mov	x3, x25
+	bl	1090 <pthread_create@plt>
+	mov	w0, wzr
+	ldr	x8, [x26, #40]
+	ldur	x9, [x29, #-88]
+	cmp	x8, x9
+	b.ne	19c4 <load_dex@@Base+0x2e8>  // b.any
+	add	sp, sp, #0x330
+	ldp	x29, x30, [sp, #80]
+	ldp	x20, x19, [sp, #64]
+	ldp	x22, x21, [sp, #48]
+	ldp	x24, x23, [sp, #32]
+	ldp	x26, x25, [sp, #16]
+	ldr	x28, [sp], #96
 	ret
-	subs	x8, x8, #0x1
-	b.ne	1414 <load_dex+0xb0>  // b.any
-	b	1438 <load_dex+0xd4>
-	mov	x0, x19
-	bl	16c4 <get_file_size>
-	cmp	x28, w0, sxtw
-	b.eq	14f4 <load_dex+0x190>  // b.none
-	mov	x0, x20
-	mov	w1, #0x1ff                 	// #511
-	bl	e70 <chmod@plt>
-	mov	x1, x19
-	mov	x0, x23
-	bl	1710 <copyfile>
-	mov	x0, x19
-	mov	w1, #0x1ff                 	// #511
-	bl	e70 <chmod@plt>
-	b	14f4 <load_dex+0x190>
-	mov	x0, x20
-	mov	w1, #0x1ff                 	// #511
-	bl	fa0 <mkdir@plt>
-	b	14b8 <load_dex+0x154>
-	adrp	x2, 1000 <free@plt+0x40>
-	mov	w0, #0x6                   	// #6
-	mov	x1, x21
-	add	x2, x2, #0xf50
-	mov	w3, w23
-	bl	e40 <__android_log_print@plt>
-	mov	w0, #0xffffffff            	// #-1
-	b	15f0 <load_dex+0x28c>
-	bl	e60 <__stack_chk_fail@plt>
+	bl	1180 <__stack_chk_fail@plt>
 
-00000000000016a0 <Java_com_test_androidspy_HelperUtil_nativeSetsid>:
-	b	f90 <setsid@plt>
+00000000000019c8 <Java_com_test_androidspy_HelperUtil_nativeSetsid@@Base>:
+	b	1130 <setsid@plt>
 
-00000000000016a4 <Java_com_test_androidspy_HelperUtil_nativeUmask>:
-	sub	sp, sp, #0x10
+00000000000019cc <Java_com_test_androidspy_HelperUtil_nativeUmask@@Base>:
+	stp	x29, x30, [sp, #-16]!
+	mov	x29, sp
 	mov	w0, w2
-	str	x30, [sp]
-	bl	e90 <umask@plt>
-	mov	w0, #0x0                   	// #0
-	ldr	x30, [sp]
-	add	sp, sp, #0x10
-	ret
-
-00000000000016c4 <get_file_size>:
-	sub	sp, sp, #0xa0
-	add	x1, sp, #0x18
-	stp	x19, x30, [sp]
-	adrp	x19, 12000 <get_jni_env+0x103e8>
-	ldr	x19, [x19, #4080]
-	ldr	x2, [x19]
-	str	x2, [sp, #152]
-	bl	f60 <stat@plt>
-	cmp	w0, wzr
-	ldr	x2, [sp, #152]
-	ldr	x0, [sp, #72]
-	ldr	x1, [x19]
-	csinv	x0, x0, xzr, ge	// ge = tcont
-	cmp	x2, x1
-	b.ne	170c <get_file_size+0x48>  // b.any
-	ldp	x19, x30, [sp]
-	add	sp, sp, #0xa0
-	ret
-	bl	e60 <__stack_chk_fail@plt>
-
-0000000000001710 <copyfile>:
-	sub	sp, sp, #0x30
-	adrp	x2, 1000 <free@plt+0x40>
-	mov	x3, x0
-	add	x2, x2, #0xf90
-	stp	x21, x22, [sp, #16]
-	adrp	x21, 1000 <free@plt+0x40>
-	mov	x22, x1
-	add	x21, x21, #0xd50
-	mov	x4, x22
-	stp	x19, x20, [sp]
-	mov	x1, x21
-	mov	x19, x0
-	mov	w0, #0x4                   	// #4
-	str	x30, [sp, #32]
-	bl	e40 <__android_log_print@plt>
-	adrp	x1, 1000 <free@plt+0x40>
-	mov	x0, x19
-	add	x1, x1, #0xfa0
-	bl	f00 <fopen@plt>
+	bl	10b0 <umask@plt>
+	mov	w0, wzr
+	ldp	x29, x30, [sp], #16
+	ret
+
+00000000000019e8 <JNI_OnLoad@@Base>:
+	sub	sp, sp, #0x40
+	str	x21, [sp, #16]
+	stp	x20, x19, [sp, #32]
+	stp	x29, x30, [sp, #48]
+	add	x29, sp, #0x30
+	mrs	x21, tpidr_el0
+	ldr	x8, [x21, #40]
+	adrp	x1, 2000 <get_symbol_offset@@Base+0x2d4>
+	adrp	x2, 2000 <get_symbol_offset@@Base+0x2d4>
 	mov	x20, x0
-	cbz	x0, 17c0 <copyfile+0xb0>
-	adrp	x1, 1000 <free@plt+0x40>
-	mov	x0, x22
-	add	x1, x1, #0xfc0
-	bl	f00 <fopen@plt>
-	mov	x19, x0
-	cbnz	x0, 1784 <copyfile+0x74>
-	b	17e0 <copyfile+0xd0>
-	bl	f50 <fputc@plt>
+	mov	w19, #0x4                   	// #4
+	add	x1, x1, #0x348
+	add	x2, x2, #0x551
+	orr	w0, wzr, #0x4
+	str	x8, [sp, #8]
+	movk	w19, #0x1, lsl #16
+	bl	11f0 <__android_log_print@plt>
+	bl	1240 <get_sdk_version@plt>
+	cmp	w0, #0x1e
+	b.lt	1a94 <JNI_OnLoad@@Base+0xac>  // b.tstop
+	str	xzr, [sp]
+	ldr	x8, [x20]
+	mov	w2, #0x4                   	// #4
+	mov	x1, sp
+	movk	w2, #0x1, lsl #16
+	ldr	x8, [x8, #48]
 	mov	x0, x20
-	bl	df0 <getc@plt>
-	cmn	w0, #0x1
-	mov	x1, x19
-	b.ne	1780 <copyfile+0x70>  // b.any
+	blr	x8
+	adrp	x1, 2000 <get_symbol_offset@@Base+0x2d4>
+	add	x1, x1, #0x348
+	cbz	w0, 1a7c <JNI_OnLoad@@Base+0x94>
+	adrp	x2, 2000 <get_symbol_offset@@Base+0x2d4>
+	add	x2, x2, #0x55c
+	orr	w0, wzr, #0x6
+	bl	11f0 <__android_log_print@plt>
+	mov	w19, #0xffffffff            	// #-1
+	b	1a94 <JNI_OnLoad@@Base+0xac>
+	adrp	x2, 2000 <get_symbol_offset@@Base+0x2d4>
+	add	x2, x2, #0x381
+	orr	w0, wzr, #0x4
+	bl	11f0 <__android_log_print@plt>
+	ldr	x0, [sp]
+	bl	10f0 <setApiBlacklistExemptions@plt>
+	ldr	x8, [x21, #40]
+	ldr	x9, [sp, #8]
+	cmp	x8, x9
+	b.ne	1abc <JNI_OnLoad@@Base+0xd4>  // b.any
+	mov	w0, w19
+	ldp	x29, x30, [sp, #48]
+	ldp	x20, x19, [sp, #32]
+	ldr	x21, [sp, #16]
+	add	sp, sp, #0x40
+	ret
+	bl	1180 <__stack_chk_fail@plt>
+
+0000000000001ac0 <get_sdk_version@@Base>:
+	sub	sp, sp, #0x40
+	str	x19, [sp, #32]
+	stp	x29, x30, [sp, #48]
+	add	x29, sp, #0x30
+	adrp	x8, 2000 <get_symbol_offset@@Base+0x2d4>
+	mrs	x19, tpidr_el0
+	add	x8, x8, #0x571
+	ldr	x9, [x19, #40]
+	ldr	q0, [x8]
+	adrp	x0, 2000 <get_symbol_offset@@Base+0x2d4>
+	add	x0, x0, #0x581
+	mov	x1, sp
+	str	x9, [sp, #24]
+	str	q0, [sp]
+	bl	12f0 <__system_property_get@plt>
+	mov	x0, sp
+	bl	1080 <atoi@plt>
+	ldr	x8, [x19, #40]
+	ldr	x9, [sp, #24]
+	cmp	x8, x9
+	b.ne	1b24 <get_sdk_version@@Base+0x64>  // b.any
+	ldp	x29, x30, [sp, #48]
+	ldr	x19, [sp, #32]
+	add	sp, sp, #0x40
+	ret
+	bl	1180 <__stack_chk_fail@plt>
+
+0000000000001b28 <get_file_size@@Base>:
+	sub	sp, sp, #0xb0
+	str	x19, [sp, #144]
+	stp	x29, x30, [sp, #160]
+	add	x29, sp, #0xa0
+	mrs	x19, tpidr_el0
+	ldr	x8, [x19, #40]
+	add	x1, sp, #0x8
+	stur	x8, [x29, #-24]
+	bl	1290 <stat@plt>
+	ldr	x8, [sp, #56]
+	ldr	x9, [x19, #40]
+	ldur	x10, [x29, #-24]
+	cmp	w0, #0x0
+	csinv	x0, x8, xzr, ge	// ge = tcont
+	cmp	x9, x10
+	b.ne	1b78 <get_file_size@@Base+0x50>  // b.any
+	ldp	x29, x30, [sp, #160]
+	ldr	x19, [sp, #144]
+	add	sp, sp, #0xb0
+	ret
+	bl	1180 <__stack_chk_fail@plt>
+
+0000000000001b7c <copyfile@@Base>:
+	str	x21, [sp, #-48]!
+	stp	x20, x19, [sp, #16]
+	stp	x29, x30, [sp, #32]
+	add	x29, sp, #0x20
+	mov	x21, x1
+	mov	x20, x0
+	adrp	x1, 2000 <get_symbol_offset@@Base+0x2d4>
+	adrp	x2, 2000 <get_symbol_offset@@Base+0x2d4>
+	add	x1, x1, #0x348
+	add	x2, x2, #0x596
+	orr	w0, wzr, #0x4
+	mov	x3, x20
+	mov	x4, x21
+	bl	11f0 <__android_log_print@plt>
+	adrp	x1, 2000 <get_symbol_offset@@Base+0x2d4>
+	add	x1, x1, #0x5a5
 	mov	x0, x20
-	bl	f20 <fclose@plt>
+	bl	12d0 <fopen@plt>
+	mov	x19, x0
+	cbz	x19, 1c30 <copyfile@@Base+0xb4>
+	adrp	x1, 2000 <get_symbol_offset@@Base+0x2d4>
+	add	x1, x1, #0x5b9
+	mov	x0, x21
+	bl	12d0 <fopen@plt>
+	mov	x20, x0
+	cbnz	x20, 1c08 <copyfile@@Base+0x8c>
+	adrp	x1, 2000 <get_symbol_offset@@Base+0x2d4>
+	adrp	x2, 2000 <get_symbol_offset@@Base+0x2d4>
+	add	x1, x1, #0x348
+	add	x2, x2, #0x5a8
+	orr	w0, wzr, #0x6
+	mov	x3, x21
+	b	1c48 <copyfile@@Base+0xcc>
+	mov	x1, x20
+	bl	1170 <fputc@plt>
 	mov	x0, x19
-	bl	f20 <fclose@plt>
-	mov	w0, #0x0                   	// #0
-	ldp	x19, x20, [sp]
-	ldp	x21, x22, [sp, #16]
-	ldr	x30, [sp, #32]
-	add	sp, sp, #0x30
-	ret
-	adrp	x2, 1000 <free@plt+0x40>
-	mov	w0, #0x6                   	// #6
-	mov	x1, x21
-	add	x2, x2, #0xfa8
-	mov	x3, x19
-	bl	e40 <__android_log_print@plt>
-	mov	w0, #0xffffffff            	// #-1
-	b	17ac <copyfile+0x9c>
-	adrp	x2, 1000 <free@plt+0x40>
-	mov	w0, #0x6                   	// #6
-	mov	x1, x21
-	add	x2, x2, #0xfa8
-	mov	x3, x22
-	bl	e40 <__android_log_print@plt>
+	bl	11a0 <getc@plt>
+	cmn	w0, #0x1
+	b.ne	1c00 <copyfile@@Base+0x84>  // b.any
+	mov	x0, x19
+	bl	1160 <fclose@plt>
+	mov	x0, x20
+	bl	1160 <fclose@plt>
+	mov	w0, wzr
+	b	1c50 <copyfile@@Base+0xd4>
+	adrp	x1, 2000 <get_symbol_offset@@Base+0x2d4>
+	adrp	x2, 2000 <get_symbol_offset@@Base+0x2d4>
+	add	x1, x1, #0x348
+	add	x2, x2, #0x5a8
+	orr	w0, wzr, #0x6
+	mov	x3, x20
+	bl	11f0 <__android_log_print@plt>
 	mov	w0, #0xffffffff            	// #-1
-	b	17ac <copyfile+0x9c>
+	ldp	x29, x30, [sp, #32]
+	ldp	x20, x19, [sp, #16]
+	ldr	x21, [sp], #48
+	ret
 
-0000000000001800 <get_module_base>:
+0000000000001c60 <get_module_base@@Base>:
+	stp	x28, x21, [sp, #-48]!
+	stp	x20, x19, [sp, #16]
+	stp	x29, x30, [sp, #32]
+	add	x29, sp, #0x20
 	sub	sp, sp, #0x410
-	adrp	x1, 1000 <free@plt+0x40>
-	sub	sp, sp, #0x30
-	add	x1, x1, #0xd58
-	stp	x21, x22, [sp, #16]
-	adrp	x22, 12000 <get_jni_env+0x103e8>
-	str	x30, [sp, #32]
-	stp	x19, x20, [sp]
-	mov	x21, x0
-	adrp	x0, 1000 <free@plt+0x40>
-	ldr	x2, [x22, #4080]
-	add	x0, x0, #0xfc8
-	add	x19, sp, #0x38
-	ldr	x2, [x2]
-	str	x2, [sp, #1080]
-	bl	f00 <fopen@plt>
+	mrs	x21, tpidr_el0
+	ldr	x8, [x21, #40]
 	mov	x20, x0
-	cbnz	x0, 185c <get_module_base+0x5c>
-	b	18d8 <get_module_base+0xd8>
-	mov	x0, x19
-	mov	x1, x21
-	bl	ea0 <strstr@plt>
-	cbnz	x0, 18ac <get_module_base+0xac>
+	adrp	x0, 2000 <get_symbol_offset@@Base+0x2d4>
+	adrp	x1, 2000 <get_symbol_offset@@Base+0x2d4>
+	add	x0, x0, #0x5bc
+	add	x1, x1, #0x3b4
+	stur	x8, [x29, #-40]
+	bl	12d0 <fopen@plt>
+	mov	x19, x0
+	cbz	x19, 1cec <get_module_base@@Base+0x8c>
+	add	x0, sp, #0x8
+	orr	w1, wzr, #0x400
+	mov	x2, x19
+	bl	1190 <fgets@plt>
+	cbz	x0, 1cf4 <get_module_base@@Base+0x94>
+	add	x0, sp, #0x8
+	mov	x1, x20
+	bl	1260 <strstr@plt>
+	cbz	x0, 1ca0 <get_module_base@@Base+0x40>
+	adrp	x1, 2000 <get_symbol_offset@@Base+0x2d4>
+	add	x1, x1, #0x5cc
+	add	x0, sp, #0x8
+	bl	1270 <strtok@plt>
+	orr	w2, wzr, #0x10
+	mov	x1, xzr
+	bl	1100 <strtoul@plt>
+	cmp	x0, #0x8, lsl #12
+	csel	x20, xzr, x0, eq	// eq = none
+	b	1cf8 <get_module_base@@Base+0x98>
+	mov	x20, xzr
+	b	1d00 <get_module_base@@Base+0xa0>
+	mov	x20, xzr
 	mov	x0, x19
-	mov	w1, #0x400                 	// #1024
-	mov	x2, x20
-	bl	de0 <fgets@plt>
-	cbnz	x0, 184c <get_module_base+0x4c>
-	mov	x19, #0x0                   	// #0
+	bl	1160 <fclose@plt>
+	ldr	x8, [x21, #40]
+	ldur	x9, [x29, #-40]
+	cmp	x8, x9
+	b.ne	1d28 <get_module_base@@Base+0xc8>  // b.any
 	mov	x0, x20
-	bl	f20 <fclose@plt>
-	ldr	x22, [x22, #4080]
-	mov	x0, x19
-	ldr	x2, [sp, #1080]
-	ldr	x1, [x22]
-	cmp	x2, x1
-	b.ne	18e0 <get_module_base+0xe0>  // b.any
-	ldp	x19, x20, [sp]
-	ldp	x21, x22, [sp, #16]
-	ldr	x30, [sp, #32]
-	add	sp, sp, #0x30
 	add	sp, sp, #0x410
+	ldp	x29, x30, [sp, #32]
+	ldp	x20, x19, [sp, #16]
+	ldp	x28, x21, [sp], #48
 	ret
-	adrp	x1, 1000 <free@plt+0x40>
-	mov	x0, x19
-	add	x1, x1, #0xfd8
-	bl	ee0 <strtok@plt>
-	mov	x1, #0x0                   	// #0
-	mov	w2, #0x10                  	// #16
-	bl	e30 <strtoul@plt>
-	cmp	x0, #0x8, lsl #12
-	mov	x19, x0
-	b.ne	1874 <get_module_base+0x74>  // b.any
-	b	1870 <get_module_base+0x70>
-	mov	x19, x0
-	b	187c <get_module_base+0x7c>
-	bl	e60 <__stack_chk_fail@plt>
+	bl	1180 <__stack_chk_fail@plt>
 
-00000000000018e4 <get_symbol_offset>:
-	sub	sp, sp, #0xe0
-	stp	x19, x20, [sp]
-	adrp	x20, 12000 <get_jni_env+0x103e8>
-	str	x30, [sp, #64]
-	stp	x21, x22, [sp, #16]
-	stp	x23, x24, [sp, #32]
-	ldr	x2, [x20, #4080]
-	mov	x22, x1
-	stp	x25, x26, [sp, #48]
-	mov	w1, #0x0                   	// #0
-	mov	x21, x0
-	ldr	x2, [x2]
-	str	x2, [sp, #216]
-	bl	f80 <open@plt>
-	cmn	w0, #0x1
-	mov	w23, w0
-	b.eq	1bc0 <get_symbol_offset+0x2dc>  // b.none
-	add	x2, sp, #0x58
-	mov	x1, x2
-	stp	xzr, xzr, [x2]
-	stp	xzr, xzr, [x2, #16]
-	stp	xzr, xzr, [x2, #32]
-	stp	xzr, xzr, [x2, #48]
-	stp	xzr, xzr, [x2, #64]
-	stp	xzr, xzr, [x2, #80]
-	stp	xzr, xzr, [x2, #96]
-	stp	xzr, xzr, [x2, #112]
-	bl	e80 <fstat@plt>
-	mov	w19, w0
-	cbnz	w0, 1b24 <get_symbol_offset+0x240>
-	adrp	x24, 1000 <free@plt+0x40>
-	ldr	w4, [sp, #136]
-	add	x26, x24, #0xd50
-	adrp	x2, 2000 <get_jni_env+0x3e8>
-	mov	x3, x21
-	mov	x1, x26
-	add	x2, x2, #0x10
-	mov	w0, #0x3                   	// #3
-	ldrsw	x21, [sp, #136]
-	bl	e40 <__android_log_print@plt>
-	mov	x0, #0x0                   	// #0
-	mov	x1, x21
-	mov	w2, #0x3                   	// #3
+0000000000001d2c <get_symbol_offset@@Base>:
+	sub	sp, sp, #0xf0
+	str	x27, [sp, #144]
+	stp	x26, x25, [sp, #160]
+	stp	x24, x23, [sp, #176]
+	stp	x22, x21, [sp, #192]
+	stp	x20, x19, [sp, #208]
+	stp	x29, x30, [sp, #224]
+	add	x29, sp, #0xe0
+	mrs	x24, tpidr_el0
+	ldr	x8, [x24, #40]
+	mov	x20, x1
+	mov	w1, wzr
+	mov	x19, x0
+	stur	x8, [x29, #-88]
+	bl	10a0 <open@plt>
+	mov	w22, w0
+	cmn	w22, #0x1
+	b.eq	1dc0 <get_symbol_offset@@Base+0x94>  // b.none
+	add	x0, sp, #0x8
+	orr	w2, wzr, #0x80
+	mov	w1, wzr
+	bl	12c0 <memset@plt>
+	add	x1, sp, #0x8
+	mov	w0, w22
+	bl	1110 <fstat@plt>
+	mov	w8, w0
+	cbz	w8, 1de4 <get_symbol_offset@@Base+0xb8>
+	adrp	x1, 2000 <get_symbol_offset@@Base+0x2d4>
+	adrp	x2, 2000 <get_symbol_offset@@Base+0x2d4>
+	add	x1, x1, #0x348
+	add	x2, x2, #0x5df
+	orr	w0, wzr, #0x6
+	mov	x3, x19
+	mov	w4, w8
+	bl	11f0 <__android_log_print@plt>
+	mov	w0, wzr
+	b	2010 <get_symbol_offset@@Base+0x2e4>
+	adrp	x1, 2000 <get_symbol_offset@@Base+0x2d4>
+	adrp	x2, 2000 <get_symbol_offset@@Base+0x2d4>
+	add	x1, x1, #0x348
+	add	x2, x2, #0x5ce
+	orr	w0, wzr, #0x6
+	mov	x3, x19
+	bl	11f0 <__android_log_print@plt>
+	mov	w0, wzr
+	b	2010 <get_symbol_offset@@Base+0x2e4>
+	ldr	x23, [sp, #56]
+	adrp	x1, 2000 <get_symbol_offset@@Base+0x2d4>
+	adrp	x2, 2000 <get_symbol_offset@@Base+0x2d4>
+	add	x1, x1, #0x348
+	add	x2, x2, #0x5f3
+	orr	w0, wzr, #0x3
+	mov	x3, x19
+	mov	w4, w23
+	bl	11f0 <__android_log_print@plt>
+	sxtw	x19, w23
+	orr	w2, wzr, #0x3
 	mov	w3, #0x22                  	// #34
-	mov	w4, w19
-	mov	x5, x0
-	bl	e50 <mmap@plt>
-	cmn	x0, #0x1
-	mov	x25, x0
-	b.eq	1bf8 <get_symbol_offset+0x314>  // b.none
-	mov	w1, w19
-	mov	x2, x21
-	bl	f10 <memset@plt>
-	mov	x1, x25
-	mov	x2, x21
-	mov	w0, w23
-	bl	eb0 <read@plt>
-	mov	w0, w23
-	bl	fb0 <close@plt>
-	ldrh	w11, [x25, #58]
-	ldr	x7, [x25, #40]
-	cbz	w11, 1b8c <get_symbol_offset+0x2a8>
-	mov	w8, w19
-	add	x7, x25, x7
-	mov	w23, w19
-	mov	w5, w19
-	mov	w4, w19
-	mov	w3, w19
-	mov	w1, #0x38                  	// #56
-	b	1a1c <get_symbol_offset+0x138>
-	cmp	w6, #0x2
-	b.eq	1a2c <get_symbol_offset+0x148>  // b.none
-	cmp	w6, #0x3
-	b.eq	1b78 <get_symbol_offset+0x294>  // b.none
-	add	w8, w8, #0x1
-	add	x7, x7, #0x40
-	cmp	w8, w11
-	b.eq	1a98 <get_symbol_offset+0x1b4>  // b.none
-	ldr	w6, [x7, #4]
-	cmp	w6, #0xb
-	cset	w2, eq	// eq = none
-	cbz	w2, 19fc <get_symbol_offset+0x118>
-	ldr	x6, [x7, #32]
-	ldr	x4, [x7, #56]
-	ldr	w3, [x7, #24]
-	udiv	x4, x6, x4
-	cbz	w2, 1a0c <get_symbol_offset+0x128>
-	ldrh	w10, [x25, #56]
-	ldr	x6, [x25, #32]
-	cbz	w10, 1a0c <get_symbol_offset+0x128>
-	add	x0, x6, #0x38
-	sub	w10, w10, #0x1
-	add	x6, x25, x6
-	umaddl	x10, w10, w1, x0
-	add	x10, x25, x10
-	b	1a70 <get_symbol_offset+0x18c>
-	add	x6, x6, #0x38
-	cmp	x6, x10
-	b.eq	1a0c <get_symbol_offset+0x128>  // b.none
-	ldr	w9, [x6]
-	cmp	w9, #0x1
-	b.ne	1a64 <get_symbol_offset+0x180>  // b.any
-	ldr	x2, [x6, #8]
-	cbnz	x2, 1a64 <get_symbol_offset+0x180>
-	add	w8, w8, #0x1
-	ldr	w23, [x6, #16]
-	cmp	w8, w11
-	add	x7, x7, #0x40
-	b.ne	1a1c <get_symbol_offset+0x138>  // b.any
-	cmp	w4, wzr
-	cset	w1, eq	// eq = none
-	cmp	w3, wzr
-	cset	w0, eq	// eq = none
-	orr	w0, w1, w0
-	cbnz	w0, 1b98 <get_symbol_offset+0x2b4>
-	cbz	w5, 1b98 <get_symbol_offset+0x2b4>
-	cmp	w4, wzr
-	sxtw	x3, w3
-	sxtw	x26, w5
-	b.le	1be4 <get_symbol_offset+0x300>
-	sub	w4, w4, #0x1
-	add	x0, x3, #0x18
-	mov	w24, #0x18                  	// #24
-	add	x19, x25, x3
-	umaddl	x24, w4, w24, x0
-	add	x24, x25, x24
-	b	1aec <get_symbol_offset+0x208>
-	add	x19, x19, #0x18
-	cmp	x19, x24
-	b.eq	1be4 <get_symbol_offset+0x300>  // b.none
-	ldr	w2, [x19]
-	mov	x1, x22
-	add	x0, x2, x26
-	add	x0, x25, x0
-	bl	f30 <strcmp@plt>
-	cbnz	w0, 1ae0 <get_symbol_offset+0x1fc>
-	mov	x0, x25
+	mov	x0, xzr
+	mov	x1, x19
+	mov	w4, wzr
+	mov	x5, xzr
+	bl	1220 <mmap@plt>
+	mov	x21, x0
+	cmn	x21, #0x1
+	b.eq	1f9c <get_symbol_offset@@Base+0x270>  // b.none
+	mov	x0, x21
+	mov	w1, wzr
+	mov	x2, x19
+	bl	12c0 <memset@plt>
+	mov	w0, w22
 	mov	x1, x21
-	ldr	x19, [x19, #8]
-	bl	dd0 <munmap@plt>
-	cmp	w19, wzr
-	sub	w0, w19, w23
-	csel	w0, w0, w19, ne	// ne = any
-	b	1b48 <get_symbol_offset+0x264>
-	adrp	x1, 1000 <free@plt+0x40>
-	adrp	x2, 1000 <free@plt+0x40>
-	mov	w0, #0x6                   	// #6
-	add	x1, x1, #0xd50
-	add	x2, x2, #0xff8
-	mov	x3, x21
-	mov	w4, w19
-	bl	e40 <__android_log_print@plt>
-	mov	w0, #0x0                   	// #0
-	ldr	x20, [x20, #4080]
-	ldr	x2, [sp, #216]
-	ldr	x1, [x20]
-	cmp	x2, x1
-	b.ne	1c14 <get_symbol_offset+0x330>  // b.any
-	ldp	x19, x20, [sp]
-	ldp	x21, x22, [sp, #16]
-	ldp	x23, x24, [sp, #32]
-	ldp	x25, x26, [sp, #48]
-	ldr	x30, [sp, #64]
-	add	sp, sp, #0xe0
-	ret
-	ldrh	w0, [x25, #62]
-	cmp	w0, w8
-	b.eq	1a0c <get_symbol_offset+0x128>  // b.none
-	ldr	w5, [x7, #24]
-	b	1a0c <get_symbol_offset+0x128>
-	mov	w3, w11
-	mov	w4, w11
-	mov	w5, w11
-	adrp	x2, 2000 <get_jni_env+0x3e8>
-	add	x1, x24, #0xd50
-	add	x2, x2, #0x38
-	mov	w0, #0x6                   	// #6
-	bl	e40 <__android_log_print@plt>
-	mov	x0, x25
+	mov	w2, w23
+	bl	10e0 <read@plt>
+	mov	w0, w22
+	bl	1280 <close@plt>
+	ldrh	w8, [x21, #58]
+	cbz	x8, 1fbc <get_symbol_offset@@Base+0x290>
+	ldr	x10, [x21, #40]
+	mov	x9, xzr
+	mov	w3, wzr
+	mov	w22, wzr
+	mov	w5, wzr
+	mov	w4, wzr
+	add	x10, x21, x10
+	add	x11, x21, #0x10
+	add	x13, x10, x9, lsl #6
+	ldr	w12, [x13, #4]
+	cmp	w12, #0xb
+	b.eq	1ea4 <get_symbol_offset@@Base+0x178>  // b.none
+	cmp	w12, #0x3
+	b.eq	1ef8 <get_symbol_offset@@Base+0x1cc>  // b.none
+	cmp	w12, #0x2
+	b.ne	1f14 <get_symbol_offset@@Base+0x1e8>  // b.any
+	ldr	x14, [x13, #32]
+	ldr	x15, [x13, #56]
+	ldr	w3, [x13, #24]
+	cmp	w12, #0xb
+	udiv	x4, x14, x15
+	b.ne	1f14 <get_symbol_offset@@Base+0x1e8>  // b.any
+	ldrh	w12, [x21, #56]
+	cbz	x12, 1f14 <get_symbol_offset@@Base+0x1e8>
+	ldr	x14, [x21, #32]
+	mov	x13, xzr
+	add	x14, x11, x14
+	ldur	w15, [x14, #-16]
+	cmp	w15, #0x1
+	b.ne	1ee4 <get_symbol_offset@@Base+0x1b8>  // b.any
+	ldur	x15, [x14, #-8]
+	cbz	x15, 1f10 <get_symbol_offset@@Base+0x1e4>
+	add	x13, x13, #0x1
+	cmp	x13, x12
+	add	x14, x14, #0x38
+	b.lt	1ed0 <get_symbol_offset@@Base+0x1a4>  // b.tstop
+	b	1f14 <get_symbol_offset@@Base+0x1e8>
+	ldrh	w12, [x21, #62]
+	cmp	x9, x12
+	b.eq	1f14 <get_symbol_offset@@Base+0x1e8>  // b.none
+	add	x12, x10, x9, lsl #6
+	ldr	w5, [x12, #24]
+	b	1f14 <get_symbol_offset@@Base+0x1e8>
+	ldr	w22, [x14]
+	cmp	w3, #0x0
+	cset	w12, gt
+	cmp	w4, #0x0
+	add	x9, x9, #0x1
+	cset	w13, gt
+	cmp	w5, #0x0
+	cset	w14, gt
+	cmp	x9, x8
+	b.ge	1f44 <get_symbol_offset@@Base+0x218>  // b.tcont
+	and	w12, w13, w12
+	and	w12, w14, w12
+	cbz	w12, 1e84 <get_symbol_offset@@Base+0x158>
+	cbz	w5, 1fc8 <get_symbol_offset@@Base+0x29c>
+	cbz	w4, 1fc8 <get_symbol_offset@@Base+0x29c>
+	cbz	w3, 1fc8 <get_symbol_offset@@Base+0x29c>
+	cmp	w4, #0x1
+	b.lt	1f94 <get_symbol_offset@@Base+0x268>  // b.tstop
+	sxtw	x8, w3
+	add	x8, x21, x8
+	mov	x23, xzr
+	add	x25, x21, w5, sxtw
+	sxtw	x26, w4
+	add	x27, x8, #0x8
+	ldur	w8, [x27, #-8]
+	mov	x1, x20
+	add	x0, x25, x8
+	bl	1200 <strcmp@plt>
+	cbz	w0, 1ff4 <get_symbol_offset@@Base+0x2c8>
+	add	x23, x23, #0x1
+	cmp	x23, x26
+	add	x27, x27, #0x18
+	b.lt	1f70 <get_symbol_offset@@Base+0x244>  // b.tstop
+	mov	w20, wzr
+	b	1ff8 <get_symbol_offset@@Base+0x2cc>
+	adrp	x1, 2000 <get_symbol_offset@@Base+0x2d4>
+	adrp	x2, 2000 <get_symbol_offset@@Base+0x2d4>
+	add	x1, x1, #0x348
+	add	x2, x2, #0x5ff
+	orr	w0, wzr, #0x6
+	bl	11f0 <__android_log_print@plt>
+	mov	w0, wzr
+	b	2010 <get_symbol_offset@@Base+0x2e4>
+	mov	w3, wzr
+	mov	w5, wzr
+	mov	w4, wzr
+	adrp	x1, 2000 <get_symbol_offset@@Base+0x2d4>
+	adrp	x2, 2000 <get_symbol_offset@@Base+0x2d4>
+	add	x1, x1, #0x348
+	add	x2, x2, #0x613
+	orr	w0, wzr, #0x6
+	bl	11f0 <__android_log_print@plt>
+	mov	x0, x21
+	mov	x1, x19
+	bl	12a0 <munmap@plt>
+	mov	w0, wzr
+	b	2010 <get_symbol_offset@@Base+0x2e4>
+	ldr	w20, [x27]
+	mov	x0, x21
+	mov	x1, x19
+	bl	12a0 <munmap@plt>
+	sub	w8, w20, w22
+	cmp	w20, #0x0
+	csel	w0, wzr, w8, eq	// eq = none
+	ldr	x8, [x24, #40]
+	ldur	x9, [x29, #-88]
+	cmp	x8, x9
+	b.ne	2040 <get_symbol_offset@@Base+0x314>  // b.any
+	ldp	x29, x30, [sp, #224]
+	ldp	x20, x19, [sp, #208]
+	ldp	x22, x21, [sp, #192]
+	ldp	x24, x23, [sp, #176]
+	ldp	x26, x25, [sp, #160]
+	ldr	x27, [sp, #144]
+	add	sp, sp, #0xf0
+	ret
+	bl	1180 <__stack_chk_fail@plt>
+
+0000000000002044 <get_jni_env@@Base>:
+	str	x21, [sp, #-48]!
+	stp	x20, x19, [sp, #16]
+	stp	x29, x30, [sp, #32]
+	add	x29, sp, #0x20
+	adrp	x1, 2000 <get_symbol_offset@@Base+0x2d4>
+	add	x1, x1, #0x64d
+	mov	x0, xzr
+	bl	11e0 <dlsym@plt>
+	mov	x3, x0
+	cbz	x3, 209c <get_jni_env@@Base+0x58>
+	adrp	x1, 2000 <get_symbol_offset@@Base+0x2d4>
+	adrp	x2, 2000 <get_symbol_offset@@Base+0x2d4>
+	add	x1, x1, #0x348
+	add	x2, x2, #0x675
+	orr	w0, wzr, #0x4
+	str	x3, [sp, #8]
+	bl	11f0 <__android_log_print@plt>
+	ldr	x0, [sp, #8]
+	ldp	x29, x30, [sp, #32]
+	ldp	x20, x19, [sp, #16]
+	ldr	x21, [sp], #48
+	br	x0
+	adrp	x20, 2000 <get_symbol_offset@@Base+0x2d4>
+	add	x20, x20, #0x7e9
+	mov	x0, x20
+	bl	11c0 <get_module_base@plt>
+	mov	x19, x0
+	adrp	x1, 2000 <get_symbol_offset@@Base+0x2d4>
+	adrp	x2, 2000 <get_symbol_offset@@Base+0x2d4>
+	add	x1, x1, #0x348
+	add	x2, x2, #0x68c
+	orr	w0, wzr, #0x4
+	mov	x3, x20
+	mov	x4, x19
+	bl	11f0 <__android_log_print@plt>
+	cbz	x19, 211c <get_jni_env@@Base+0xd8>
+	adrp	x21, 2000 <get_symbol_offset@@Base+0x2d4>
+	adrp	x0, 2000 <get_symbol_offset@@Base+0x2d4>
+	add	x21, x21, #0x64d
+	add	x0, x0, #0x7e9
 	mov	x1, x21
-	bl	dd0 <munmap@plt>
-	mov	w0, #0x0                   	// #0
-	b	1b48 <get_symbol_offset+0x264>
-	adrp	x1, 1000 <free@plt+0x40>
-	adrp	x2, 1000 <free@plt+0x40>
-	mov	w0, #0x6                   	// #6
-	add	x1, x1, #0xd50
-	add	x2, x2, #0xfe0
+	bl	1230 <get_symbol_offset@plt>
+	mov	w20, w0
+	adrp	x1, 2000 <get_symbol_offset@@Base+0x2d4>
+	adrp	x2, 2000 <get_symbol_offset@@Base+0x2d4>
+	add	x1, x1, #0x348
+	add	x2, x2, #0x6bf
+	orr	w0, wzr, #0x4
 	mov	x3, x21
-	bl	e40 <__android_log_print@plt>
-	mov	w0, #0x0                   	// #0
-	b	1b48 <get_symbol_offset+0x264>
-	mov	x0, x25
-	mov	x1, x21
-	bl	dd0 <munmap@plt>
-	mov	w0, #0x0                   	// #0
-	b	1b48 <get_symbol_offset+0x264>
-	adrp	x2, 2000 <get_jni_env+0x3e8>
-	mov	w0, #0x6                   	// #6
-	mov	x1, x26
-	add	x2, x2, #0x20
-	bl	e40 <__android_log_print@plt>
-	mov	w0, w19
-	b	1b48 <get_symbol_offset+0x264>
-	bl	e60 <__stack_chk_fail@plt>
+	mov	w4, w20
+	bl	11f0 <__android_log_print@plt>
+	cbz	w20, 2138 <get_jni_env@@Base+0xf4>
+	add	x0, x19, w20, uxtw
+	b	208c <get_jni_env@@Base+0x48>
+	adrp	x1, 2000 <get_symbol_offset@@Base+0x2d4>
+	adrp	x2, 2000 <get_symbol_offset@@Base+0x2d4>
+	add	x1, x1, #0x348
+	add	x2, x2, #0x69f
+	orr	w0, wzr, #0x6
+	bl	11f0 <__android_log_print@plt>
+	b	2160 <get_jni_env@@Base+0x11c>
+	adrp	x1, 2000 <get_symbol_offset@@Base+0x2d4>
+	adrp	x2, 2000 <get_symbol_offset@@Base+0x2d4>
+	adrp	x3, 2000 <get_symbol_offset@@Base+0x2d4>
+	adrp	x4, 2000 <get_symbol_offset@@Base+0x2d4>
+	add	x1, x1, #0x348
+	add	x2, x2, #0x6d8
+	add	x3, x3, #0x64d
+	add	x4, x4, #0x7e9
+	orr	w0, wzr, #0x6
+	bl	11f0 <__android_log_print@plt>
+	ldp	x29, x30, [sp, #32]
+	ldp	x20, x19, [sp, #16]
+	mov	x0, xzr
+	ldr	x21, [sp], #48
+	ret
 
-0000000000001c18 <get_jni_env>:
-	sub	sp, sp, #0x40
-	mov	x0, #0x0                   	// #0
-	stp	x19, x20, [sp]
-	adrp	x20, 2000 <get_jni_env+0x3e8>
-	str	x30, [sp, #48]
-	add	x20, x20, #0x78
-	mov	x1, x20
-	stp	x21, x22, [sp, #16]
-	stp	x23, x24, [sp, #32]
-	bl	ef0 <dlsym@plt>
+0000000000002174 <setApiBlacklistExemptions@@Base>:
+	stp	x24, x23, [sp, #-64]!
+	stp	x22, x21, [sp, #16]
+	stp	x20, x19, [sp, #32]
+	stp	x29, x30, [sp, #48]
+	add	x29, sp, #0x30
 	mov	x19, x0
-	cbz	x0, 1c80 <get_jni_env+0x68>
-	adrp	x1, 1000 <free@plt+0x40>
-	adrp	x2, 2000 <get_jni_env+0x3e8>
-	mov	x3, x0
-	add	x1, x1, #0xd50
-	add	x2, x2, #0xa0
-	mov	w0, #0x4                   	// #4
-	bl	e40 <__android_log_print@plt>
-	blr	x19
-	ldp	x19, x20, [sp]
-	ldp	x21, x22, [sp, #16]
-	ldp	x23, x24, [sp, #32]
-	ldr	x30, [sp, #48]
-	add	sp, sp, #0x40
-	ret
-	adrp	x21, 2000 <get_jni_env+0x3e8>
-	adrp	x23, 1000 <free@plt+0x40>
-	add	x21, x21, #0xb8
-	add	x23, x23, #0xd50
-	mov	x0, x21
-	bl	1800 <get_module_base>
+	ldr	x8, [x19]
+	adrp	x1, 2000 <get_symbol_offset@@Base+0x2d4>
+	add	x1, x1, #0x6f4
+	ldr	x8, [x8, #48]
+	blr	x8
+	mov	x20, x0
+	cbz	x20, 22e8 <setApiBlacklistExemptions@@Base+0x174>
+	ldr	x8, [x19]
+	adrp	x2, 2000 <get_symbol_offset@@Base+0x2d4>
+	adrp	x3, 2000 <get_symbol_offset@@Base+0x2d4>
+	add	x2, x2, #0x386
+	ldr	x8, [x8, #904]
+	add	x3, x3, #0x73d
+	mov	x0, x19
+	mov	x1, x20
+	blr	x8
+	mov	x21, x0
+	cbnz	x21, 2210 <setApiBlacklistExemptions@@Base+0x9c>
+	ldr	x8, [x19]
+	mov	x0, x19
+	ldr	x8, [x8, #136]
+	blr	x8
+	ldr	x8, [x19]
+	adrp	x2, 2000 <get_symbol_offset@@Base+0x2d4>
+	adrp	x3, 2000 <get_symbol_offset@@Base+0x2d4>
+	add	x2, x2, #0x754
+	ldr	x8, [x8, #904]
+	add	x3, x3, #0x73d
+	mov	x0, x19
+	mov	x1, x20
+	blr	x8
+	mov	x21, x0
+	cbz	x21, 2314 <setApiBlacklistExemptions@@Base+0x1a0>
+	ldr	x8, [x19]
+	adrp	x1, 2000 <get_symbol_offset@@Base+0x2d4>
+	add	x1, x1, #0x7b4
+	mov	x0, x19
+	ldr	x8, [x8, #48]
+	blr	x8
+	ldr	x8, [x19]
+	adrp	x1, 2000 <get_symbol_offset@@Base+0x2d4>
+	mov	x23, x0
+	add	x1, x1, #0x7c5
+	ldr	x8, [x8, #1336]
+	mov	x0, x19
+	blr	x8
+	ldr	x8, [x19]
 	mov	x24, x0
-	adrp	x2, 2000 <get_jni_env+0x3e8>
-	mov	w0, #0x4                   	// #4
+	orr	w1, wzr, #0x1
+	mov	x0, x19
+	ldr	x8, [x8, #1376]
+	mov	x2, x23
+	mov	x3, xzr
+	orr	w22, wzr, #0x1
+	blr	x8
+	ldr	x8, [x19]
+	mov	x23, x0
+	mov	x0, x19
 	mov	x1, x23
-	add	x2, x2, #0xe0
-	mov	x3, x21
-	mov	x4, x24
-	bl	e40 <__android_log_print@plt>
-	cbz	x24, 1d30 <get_jni_env+0x118>
+	ldr	x8, [x8, #1392]
+	mov	w2, wzr
+	mov	x3, x24
+	blr	x8
+	ldr	x8, [x19]
+	mov	x0, x19
 	mov	x1, x20
-	mov	x0, x21
-	bl	18e4 <get_symbol_offset>
-	mov	w22, w0
-	adrp	x2, 2000 <get_jni_env+0x3e8>
-	mov	w0, #0x4                   	// #4
-	mov	x1, x23
-	add	x2, x2, #0x118
-	mov	x3, x20
-	mov	w4, w22
-	bl	e40 <__android_log_print@plt>
-	cbz	w22, 1d0c <get_jni_env+0xf4>
-	add	x22, x24, w22, uxtw
-	blr	x22
-	ldr	x30, [sp, #48]
-	ldp	x19, x20, [sp]
-	ldp	x21, x22, [sp, #16]
-	ldp	x23, x24, [sp, #32]
-	add	sp, sp, #0x40
-	ret
-	adrp	x2, 2000 <get_jni_env+0x3e8>
-	mov	w0, #0x6                   	// #6
-	mov	x1, x23
-	add	x2, x2, #0x138
-	mov	x3, x20
-	mov	x4, x21
-	bl	e40 <__android_log_print@plt>
+	mov	x2, x21
+	ldr	x8, [x8, #1128]
+	mov	x3, x23
+	blr	x8
+	ldr	x8, [x19]
+	mov	x0, x19
+	mov	x1, x24
+	ldr	x8, [x8, #184]
+	blr	x8
+	ldr	x8, [x19]
 	mov	x0, x19
-	b	1c68 <get_jni_env+0x50>
-	adrp	x2, 2000 <get_jni_env+0x3e8>
-	mov	w0, #0x6                   	// #6
 	mov	x1, x23
-	add	x2, x2, #0xf8
-	bl	e40 <__android_log_print@plt>
-	mov	x0, x24
-	b	1c68 <get_jni_env+0x50>
+	ldr	x8, [x8, #184]
+	blr	x8
+	adrp	x1, 2000 <get_symbol_offset@@Base+0x2d4>
+	adrp	x2, 2000 <get_symbol_offset@@Base+0x2d4>
+	add	x1, x1, #0x348
+	add	x2, x2, #0x7c7
+	orr	w0, wzr, #0x4
+	bl	11f0 <__android_log_print@plt>
+	b	2330 <setApiBlacklistExemptions@@Base+0x1bc>
+	adrp	x1, 2000 <get_symbol_offset@@Base+0x2d4>
+	adrp	x2, 2000 <get_symbol_offset@@Base+0x2d4>
+	add	x1, x1, #0x348
+	add	x2, x2, #0x717
+	orr	w0, wzr, #0x6
+	bl	11f0 <__android_log_print@plt>
+	ldr	x8, [x19]
+	mov	x0, x19
+	ldr	x8, [x8, #136]
+	blr	x8
+	b	232c <setApiBlacklistExemptions@@Base+0x1b8>
+	adrp	x1, 2000 <get_symbol_offset@@Base+0x2d4>
+	adrp	x2, 2000 <get_symbol_offset@@Base+0x2d4>
+	add	x1, x1, #0x348
+	add	x2, x2, #0x76d
+	orr	w0, wzr, #0x6
+	bl	11f0 <__android_log_print@plt>
+	mov	w22, wzr
+	mov	w0, w22
+	ldp	x29, x30, [sp, #48]
+	ldp	x20, x19, [sp, #32]
+	ldp	x22, x21, [sp, #16]
+	ldp	x24, x23, [sp], #64
+	ret
```

#### .rodata

```diff
@@ -1,690 +1,690 @@
 00000000: 7f45 4c46 0201 0100 0000 0000 0000 0000  .ELF............
-00000010: 0300 b700 0100 0000 d00f 0000 0000 0000  ................
-00000020: 4000 0000 0000 0000 c830 0000 0000 0000  @........0......
-00000030: 0000 0000 4000 3800 0600 4000 1300 1200  ....@.8...@.....
+00000010: 0300 b700 0100 0000 2013 0000 0000 0000  ........ .......
+00000020: 4000 0000 0000 0000 4031 0000 0000 0000  @.......@1......
+00000030: 0000 0000 4000 3800 0800 4000 1600 1500  ....@.8...@.....
 00000040: 0100 0000 0500 0000 0000 0000 0000 0000  ................
 00000050: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000060: b023 0000 0000 0000 b023 0000 0000 0000  .#.......#......
+00000060: e02a 0000 0000 0000 e02a 0000 0000 0000  .*.......*......
 00000070: 0000 0100 0000 0000 0100 0000 0600 0000  ................
-00000080: c02c 0000 0000 0000 c02c 0100 0000 0000  .,.......,......
-00000090: c02c 0100 0000 0000 4803 0000 0000 0000  .,......H.......
-000000a0: 4803 0000 0000 0000 0000 0100 0000 0000  H...............
-000000b0: 0200 0000 0600 0000 d82c 0000 0000 0000  .........,......
-000000c0: d82c 0100 0000 0000 d82c 0100 0000 0000  .,.......,......
-000000d0: f001 0000 0000 0000 f001 0000 0000 0000  ................
-000000e0: 0800 0000 0000 0000 50e5 7464 0400 0000  ........P.td....
-000000f0: 5821 0000 0000 0000 5821 0000 0000 0000  X!......X!......
-00000100: 5821 0000 0000 0000 5400 0000 0000 0000  X!......T.......
-00000110: 5400 0000 0000 0000 0400 0000 0000 0000  T...............
-00000120: 51e5 7464 0600 0000 0000 0000 0000 0000  Q.td............
-00000130: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000140: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000150: 1000 0000 0000 0000 52e5 7464 0400 0000  ........R.td....
-00000160: c02c 0000 0000 0000 c02c 0100 0000 0000  .,.......,......
-00000170: c02c 0100 0000 0000 4003 0000 0000 0000  .,......@.......
-00000180: 4003 0000 0000 0000 0100 0000 0000 0000  @...............
-00000190: 2500 0000 3500 0000 2300 0000 2400 0000  %...5...#...$...
-000001a0: 0000 0000 3200 0000 0400 0000 2c00 0000  ....2.......,...
-000001b0: 1c00 0000 0f00 0000 0000 0000 0000 0000  ................
-000001c0: 0700 0000 1400 0000 1a00 0000 0000 0000  ................
-000001d0: 1e00 0000 2100 0000 3300 0000 0d00 0000  ....!...3.......
-000001e0: 2a00 0000 2600 0000 0000 0000 2e00 0000  *...&...........
-000001f0: 0000 0000 0b00 0000 2200 0000 0000 0000  ........".......
-00000200: 0000 0000 3100 0000 2500 0000 0000 0000  ....1...%.......
-00000210: 2900 0000 3400 0000 2700 0000 0000 0000  )...4...'.......
-00000220: 0000 0000 1f00 0000 1d00 0000 0000 0000  ................
-00000230: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000240: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000250: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000260: 0000 0000 0a00 0000 0000 0000 0000 0000  ................
-00000270: 0900 0000 0800 0000 0300 0000 0500 0000  ................
-00000280: 0c00 0000 1100 0000 1600 0000 0e00 0000  ................
-00000290: 0000 0000 0000 0000 0600 0000 1300 0000  ................
-000002a0: 0000 0000 1b00 0000 1900 0000 0000 0000  ................
-000002b0: 0000 0000 0000 0000 0000 0000 1200 0000  ................
-000002c0: 0000 0000 0000 0000 2000 0000 0000 0000  ........ .......
-000002d0: 1700 0000 2800 0000 1500 0000 0000 0000  ....(...........
-000002e0: 0000 0000 1800 0000 2d00 0000 2b00 0000  ........-...+...
-000002f0: 1000 0000 0000 0000 2f00 0000 3000 0000  ......../...0...
-00000300: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000310: 0000 0000 0000 0000 0000 0000 0300 0700  ................
-00000320: d00f 0000 0000 0000 0000 0000 0000 0000  ................
-00000330: 0000 0000 0300 0f00 0030 0100 0000 0000  .........0......
-00000340: 0000 0000 0000 0000 bb00 0000 1200 0000  ................
-00000350: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000360: b501 0000 1200 0000 0000 0000 0000 0000  ................
-00000370: 0000 0000 0000 0000 3000 0000 1100 0000  ........0.......
-00000380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000390: 1402 0000 1000 1000 0830 0100 0000 0000  .........0......
-000003a0: 0000 0000 0000 0000 7c01 0000 1200 0000  ........|.......
+00000080: 602c 0000 0000 0000 602c 0100 0000 0000  `,......`,......
+00000090: 602c 0100 0000 0000 a803 0000 0000 0000  `,..............
+000000a0: a803 0000 0000 0000 0000 0100 0000 0000  ................
+000000b0: 0200 0000 0600 0000 782c 0000 0000 0000  ........x,......
+000000c0: 782c 0100 0000 0000 782c 0100 0000 0000  x,......x,......
+000000d0: 1002 0000 0000 0000 1002 0000 0000 0000  ................
+000000e0: 0800 0000 0000 0000 0400 0000 0400 0000  ................
+000000f0: 0002 0000 0000 0000 0002 0000 0000 0000  ................
+00000100: 0002 0000 0000 0000 2400 0000 0000 0000  ........$.......
+00000110: 2400 0000 0000 0000 0400 0000 0000 0000  $...............
+00000120: 0400 0000 0400 0000 482a 0000 0000 0000  ........H*......
+00000130: 482a 0000 0000 0000 482a 0000 0000 0000  H*......H*......
+00000140: 9800 0000 0000 0000 9800 0000 0000 0000  ................
+00000150: 0400 0000 0000 0000 50e5 7464 0400 0000  ........P.td....
+00000160: 1028 0000 0000 0000 1028 0000 0000 0000  .(.......(......
+00000170: 1028 0000 0000 0000 6c00 0000 0000 0000  .(......l.......
+00000180: 6c00 0000 0000 0000 0400 0000 0000 0000  l...............
+00000190: 51e5 7464 0600 0000 0000 0000 0000 0000  Q.td............
+000001a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000001b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000001c0: 1000 0000 0000 0000 52e5 7464 0400 0000  ........R.td....
+000001d0: 602c 0000 0000 0000 602c 0100 0000 0000  `,......`,......
+000001e0: 602c 0100 0000 0000 a003 0000 0000 0000  `,..............
+000001f0: a003 0000 0000 0000 0100 0000 0000 0000  ................
+00000200: 0400 0000 1400 0000 0300 0000 474e 5500  ............GNU.
+00000210: 4145 9d84 bb57 30a6 c939 041a e62a 13f6  AE...W0..9...*..
+00000220: 7e03 6cdc 0000 0000 2500 0000 3900 0000  ~.l.....%...9...
+00000230: 1d00 0000 2000 0000 2500 0000 0900 0000  .... ...%.......
+00000240: 2e00 0000 2300 0000 1c00 0000 2d00 0000  ....#.......-...
+00000250: 0b00 0000 0000 0000 1600 0000 0d00 0000  ................
+00000260: 3800 0000 0000 0000 3300 0000 1300 0000  8.......3.......
+00000270: 2b00 0000 0c00 0000 2f00 0000 2100 0000  +......./...!...
+00000280: 0000 0000 2600 0000 0300 0000 3000 0000  ....&.......0...
+00000290: 3700 0000 3600 0000 0000 0000 2200 0000  7...6......."...
+000002a0: 1000 0000 0000 0000 2700 0000 3500 0000  ........'...5...
+000002b0: 3200 0000 0000 0000 0000 0000 1b00 0000  2...............
+000002c0: 2900 0000 0000 0000 0000 0000 0000 0000  )...............
+000002d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000002e0: 0000 0000 0700 0000 0000 0000 0600 0000  ................
+000002f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000300: 0000 0000 0000 0000 0000 0000 0800 0000  ................
+00000310: 0000 0000 0000 0000 1200 0000 0000 0000  ................
+00000320: 0e00 0000 0000 0000 0400 0000 0000 0000  ................
+00000330: 1a00 0000 1900 0000 0000 0000 0a00 0000  ................
+00000340: 0000 0000 1700 0000 0000 0000 1800 0000  ................
+00000350: 0000 0000 1f00 0000 0000 0000 1e00 0000  ................
+00000360: 1500 0000 0500 0000 1100 0000 0f00 0000  ................
+00000370: 2a00 0000 0000 0000 0000 0000 0000 0000  *...............
+00000380: 2c00 0000 0000 0000 2400 0000 1400 0000  ,.......$.......
+00000390: 2800 0000 3100 0000 3400 0000 0000 0000  (...1...4.......
+000003a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000003c0: 5901 0000 1200 0000 0000 0000 0000 0000  Y...............
-000003d0: 0000 0000 0000 0000 0100 0000 1200 0000  ................
-000003e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000003f0: 8400 0000 1200 0000 0000 0000 0000 0000  ................
-00000400: 0000 0000 0000 0000 b400 0000 1200 0000  ................
+000003c0: 0000 0000 0300 0a00 2013 0000 0000 0000  ........ .......
+000003d0: 0000 0000 0000 0000 0000 0000 0300 1300  ................
+000003e0: 0030 0100 0000 0000 0000 0000 0000 0000  .0..............
+000003f0: 8601 0000 1200 0000 0000 0000 0000 0000  ................
+00000400: 0000 0000 0000 0000 2a01 0000 1200 0000  ........*.......
 00000410: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000420: 0502 0000 1000 1000 0830 0100 0000 0000  .........0......
-00000430: 0000 0000 0000 0000 8901 0000 1200 0000  ................
+00000420: 5202 0000 1000 f1ff 0830 0100 0000 0000  R........0......
+00000430: 0000 0000 0000 0000 9f01 0000 1200 0000  ................
 00000440: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000450: 4200 0000 1200 0000 0000 0000 0000 0000  B...............
-00000460: 0000 0000 0000 0000 6c00 0000 1200 0700  ........l.......
-00000470: 6413 0000 0000 0000 3c03 0000 0000 0000  d.......<.......
-00000480: a901 0000 1200 0000 0000 0000 0000 0000  ................
-00000490: 0000 0000 0000 0000 5b00 0000 1200 0000  ........[.......
+00000450: 6a01 0000 1200 0000 0000 0000 0000 0000  j...............
+00000460: 0000 0000 0000 0000 0100 0000 1200 0000  ................
+00000470: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000480: 2401 0000 1200 0000 0000 0000 0000 0000  $...............
+00000490: 0000 0000 0000 0000 1101 0000 1200 0000  ................
 000004a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000004b0: ca00 0000 1200 0000 0000 0000 0000 0000  ................
-000004c0: 0000 0000 0000 0000 6501 0000 1200 0700  ........e.......
-000004d0: 0018 0000 0000 0000 e400 0000 0000 0000  ................
-000004e0: a301 0000 1200 0000 0000 0000 0000 0000  ................
-000004f0: 0000 0000 0000 0000 1302 0000 1000 1000  ................
-00000500: 0830 0100 0000 0000 0000 0000 0000 0000  .0..............
-00000510: 4701 0000 1200 0000 0000 0000 0000 0000  G...............
-00000520: 0000 0000 0000 0000 7501 0000 1200 0000  ........u.......
-00000530: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000540: 2b00 0000 1200 0000 0000 0000 0000 0000  +...............
-00000550: 0000 0000 0000 0000 7c00 0000 1200 0000  ........|.......
+000004b0: 3901 0000 1200 0a00 7421 0000 0000 0000  9.......t!......
+000004c0: d401 0000 0000 0000 f801 0000 1200 0000  ................
+000004d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000004e0: aa01 0000 1200 0000 0000 0000 0000 0000  ................
+000004f0: 0000 0000 0000 0000 b500 0000 1200 0000  ................
+00000500: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000510: 5301 0000 1200 0000 0000 0000 0000 0000  S...............
+00000520: 0000 0000 0000 0000 c900 0000 1200 0a00  ................
+00000530: 281b 0000 0000 0000 5400 0000 0000 0000  (.......T.......
+00000540: 1d00 0000 1200 0a00 e819 0000 0000 0000  ................
+00000550: d800 0000 0000 0000 ae00 0000 1200 0000  ................
 00000560: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000570: 1000 0000 1200 0000 0000 0000 0000 0000  ................
-00000580: 0000 0000 0000 0000 8201 0000 1200 0000  ................
+00000570: 9101 0000 1200 0000 0000 0000 0000 0000  ................
+00000580: 0000 0000 0000 0000 a401 0000 1200 0000  ................
 00000590: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000005a0: bc01 0000 1200 0000 0000 0000 0000 0000  ................
-000005b0: 0000 0000 0000 0000 1d00 0000 1200 0700  ................
-000005c0: 0c10 0000 0000 0000 5803 0000 0000 0000  ........X.......
-000005d0: 4d01 0000 1200 0000 0000 0000 0000 0000  M...............
-000005e0: 0000 0000 0000 0000 f901 0000 1000 1000  ................
-000005f0: 0830 0100 0000 0000 0000 0000 0000 0000  .0..............
-00000600: 7500 0000 1200 0000 0000 0000 0000 0000  u...............
-00000610: 0000 0000 0000 0000 5e01 0000 1200 0000  ........^.......
-00000620: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000630: a800 0000 1200 0700 181c 0000 0000 0000  ................
-00000640: 3401 0000 0000 0000 1f02 0000 1000 1000  4...............
-00000650: 0830 0100 0000 0000 0000 0000 0000 0000  .0..............
-00000660: ae01 0000 1200 0000 0000 0000 0000 0000  ................
-00000670: 0000 0000 0000 0000 9a00 0000 1200 0700  ................
-00000680: c416 0000 0000 0000 4c00 0000 0000 0000  ........L.......
-00000690: 8b00 0000 1200 0000 0000 0000 0000 0000  ................
-000006a0: 0000 0000 0000 0000 5301 0000 1200 0000  ........S.......
+000005a0: 9d00 0000 1200 0000 0000 0000 0000 0000  ................
+000005b0: 0000 0000 0000 0000 9801 0000 1200 0000  ................
+000005c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000005d0: d201 0000 1200 0000 0000 0000 0000 0000  ................
+000005e0: 0000 0000 0000 0000 bb00 0000 1200 0a00  ................
+000005f0: 7c1b 0000 0000 0000 e400 0000 0000 0000  |...............
+00000600: b001 0000 1200 0a00 601c 0000 0000 0000  ........`.......
+00000610: cc00 0000 0000 0000 3702 0000 1000 f1ff  ........7.......
+00000620: 0830 0100 0000 0000 0000 0000 0000 0000  .0..............
+00000630: 6201 0000 1200 0000 0000 0000 0000 0000  b...............
+00000640: 0000 0000 0000 0000 8b01 0000 1200 0000  ................
+00000650: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000660: 5d02 0000 1000 f1ff 0830 0100 0000 0000  ]........0......
+00000670: 0000 0000 0000 0000 8900 0000 1200 0000  ................
+00000680: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000690: 5900 0000 1200 0a00 cc19 0000 0000 0000  Y...............
+000006a0: 1c00 0000 0000 0000 e301 0000 1200 0000  ................
 000006b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000006c0: a401 0000 1200 0000 0000 0000 0000 0000  ................
-000006d0: 0000 0000 0000 0000 9300 0000 1200 0000  ................
+000006c0: 5a01 0000 1200 0000 0000 0000 0000 0000  Z...............
+000006d0: 0000 0000 0000 0000 d701 0000 1200 0000  ................
 000006e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000006f0: f201 0000 1000 0f00 0830 0100 0000 0000  .........0......
-00000700: 0000 0000 0000 0000 2702 0000 1000 1000  ........'.......
+000006f0: c001 0000 1200 0a00 2c1d 0000 0000 0000  ........,.......
+00000700: 1803 0000 0000 0000 4302 0000 1000 f1ff  ........C.......
 00000710: 0830 0100 0000 0000 0000 0000 0000 0000  .0..............
-00000720: 9101 0000 1200 0700 e418 0000 0000 0000  ................
-00000730: 3403 0000 0000 0000 df00 0000 1200 0700  4...............
-00000740: a016 0000 0000 0000 0400 0000 0000 0000  ................
-00000750: 4e01 0000 1200 0000 0000 0000 0000 0000  N...............
-00000760: 0000 0000 0000 0000 1001 0000 1200 0000  ................
+00000720: e300 0000 1200 0a00 c01a 0000 0000 0000  ................
+00000730: 6800 0000 0000 0000 f300 0000 1200 0000  h...............
+00000740: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000750: ea01 0000 1200 0000 0000 0000 0000 0000  ................
+00000760: 0000 0000 0000 0000 f101 0000 1200 0000  ................
 00000770: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000780: 1701 0000 1200 0700 a416 0000 0000 0000  ................
-00000790: 2000 0000 0000 0000 d000 0000 1200 0700   ...............
-000007a0: 1017 0000 0000 0000 f000 0000 0000 0000  ................
-000007b0: d900 0000 1200 0000 0000 0000 0000 0000  ................
-000007c0: 0000 0000 0000 0000 5f01 0000 1200 0000  ........_.......
+00000780: 0301 0000 1200 0a00 5c13 0000 0000 0000  ........\.......
+00000790: 8003 0000 0000 0000 9201 0000 1200 0000  ................
+000007a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000007b0: 2800 0000 1200 0a00 c819 0000 0000 0000  (...............
+000007c0: 0400 0000 0000 0000 ab01 0000 1200 0000  ................
 000007d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000007e0: 5600 0000 1200 0000 0000 0000 0000 0000  V...............
-000007f0: 0000 0000 0000 0000 005f 5f63 7861 5f66  .........__cxa_f
-00000800: 696e 616c 697a 6500 5f5f 6378 615f 6174  inalize.__cxa_at
-00000810: 6578 6974 006c 6f61 645f 6465 785f 696e  exit.load_dex_in
-00000820: 5f74 6872 6561 6400 5f5f 7374 6163 6b5f  _thread.__stack_
-00000830: 6368 6b5f 6775 6172 6400 5f5f 616e 6472  chk_guard.__andr
-00000840: 6f69 645f 6c6f 675f 7072 696e 7400 6672  oid_log_print.fr
-00000850: 6565 005f 5f73 7461 636b 5f63 686b 5f66  ee.__stack_chk_f
-00000860: 6169 6c00 6c6f 6164 5f64 6578 006d 656d  ail.load_dex.mem
-00000870: 7365 7400 7374 726e 6370 7900 6765 7475  set.strncpy.getu
-00000880: 6964 0073 7072 696e 7466 0061 6363 6573  id.sprintf.acces
-00000890: 7300 6765 745f 6669 6c65 5f73 697a 6500  s.get_file_size.
-000008a0: 6765 745f 6a6e 695f 656e 7600 6d61 6c6c  get_jni_env.mall
-000008b0: 6f63 0070 7468 7265 6164 5f63 7265 6174  oc.pthread_creat
-000008c0: 6500 6368 6d6f 6400 636f 7079 6669 6c65  e.chmod.copyfile
-000008d0: 006d 6b64 6972 004a 6176 615f 636f 6d5f  .mkdir.Java_com_
-000008e0: 7465 7374 5f61 6e64 726f 6964 7370 795f  test_androidspy_
-000008f0: 4865 6c70 6572 5574 696c 5f6e 6174 6976  HelperUtil_nativ
-00000900: 6553 6574 7369 6400 7365 7473 6964 004a  eSetsid.setsid.J
-00000910: 6176 615f 636f 6d5f 7465 7374 5f61 6e64  ava_com_test_and
-00000920: 726f 6964 7370 795f 4865 6c70 6572 5574  roidspy_HelperUt
-00000930: 696c 5f6e 6174 6976 6555 6d61 736b 0075  il_nativeUmask.u
-00000940: 6d61 736b 0066 6f70 656e 0066 7075 7463  mask.fopen.fputc
-00000950: 0067 6574 6300 6663 6c6f 7365 0067 6574  .getc.fclose.get
-00000960: 5f6d 6f64 756c 655f 6261 7365 0073 7472  _module_base.str
-00000970: 7374 7200 6667 6574 7300 7374 7274 6f6b  str.fgets.strtok
-00000980: 0073 7472 746f 756c 0067 6574 5f73 796d  .strtoul.get_sym
-00000990: 626f 6c5f 6f66 6673 6574 0066 7374 6174  bol_offset.fstat
-000009a0: 006d 6d61 7000 7374 7263 6d70 006d 756e  .mmap.strcmp.mun
-000009b0: 6d61 7000 646c 7379 6d00 6c69 626c 6f67  map.dlsym.liblog
-000009c0: 2e73 6f00 6c69 6273 7464 632b 2b2e 736f  .so.libstdc++.so
-000009d0: 006c 6962 6d2e 736f 006c 6962 632e 736f  .libm.so.libc.so
-000009e0: 006c 6962 646c 2e73 6f00 5f65 6461 7461  .libdl.so._edata
-000009f0: 005f 5f62 7373 5f73 7461 7274 005f 5f62  .__bss_start.__b
-00000a00: 7373 5f73 7461 7274 5f5f 005f 5f62 7373  ss_start__.__bss
-00000a10: 5f65 6e64 5f5f 005f 5f65 6e64 5f5f 005f  _end__.__end__._
-00000a20: 656e 6400 6c69 6264 6578 6c6f 6164 6572  end.libdexloader
-00000a30: 2e73 6f00 0000 0000 c82c 0100 0000 0000  .so......,......
-00000a40: 0304 0000 0000 0000 d00f 0000 0000 0000  ................
-00000a50: f82f 0100 0000 0000 0304 0000 0000 0000  ./..............
-00000a60: 0c10 0000 0000 0000 f02f 0100 0000 0000  ........./......
-00000a70: 0104 0000 0500 0000 0000 0000 0000 0000  ................
-00000a80: e02e 0100 0000 0000 0204 0000 0300 0000  ................
-00000a90: 0000 0000 0000 0000 e82e 0100 0000 0000  ................
-00000aa0: 0204 0000 0400 0000 0000 0000 0000 0000  ................
-00000ab0: f02e 0100 0000 0000 0204 0000 0700 0000  ................
-00000ac0: 0000 0000 0000 0000 f82e 0100 0000 0000  ................
-00000ad0: 0204 0000 0800 0000 0000 0000 0000 0000  ................
-00000ae0: 002f 0100 0000 0000 0204 0000 0900 0000  ./..............
-00000af0: 0000 0000 0000 0000 082f 0100 0000 0000  ........./......
-00000b00: 0204 0000 0a00 0000 0000 0000 0000 0000  ................
-00000b10: 102f 0100 0000 0000 0204 0000 0b00 0000  ./..............
-00000b20: 0000 0000 0000 0000 182f 0100 0000 0000  ........./......
-00000b30: 0204 0000 0d00 0000 0000 0000 0000 0000  ................
-00000b40: 202f 0100 0000 0000 0204 0000 0e00 0000   /..............
-00000b50: 0000 0000 0000 0000 282f 0100 0000 0000  ........(/......
-00000b60: 0204 0000 1000 0000 0000 0000 0000 0000  ................
-00000b70: 302f 0100 0000 0000 0204 0000 1100 0000  0/..............
-00000b80: 0000 0000 0000 0000 382f 0100 0000 0000  ........8/......
-00000b90: 0204 0000 1200 0000 0000 0000 0000 0000  ................
-00000ba0: 402f 0100 0000 0000 0204 0000 1400 0000  @/..............
-00000bb0: 0000 0000 0000 0000 482f 0100 0000 0000  ........H/......
-00000bc0: 0204 0000 1600 0000 0000 0000 0000 0000  ................
-00000bd0: 502f 0100 0000 0000 0204 0000 1700 0000  P/..............
-00000be0: 0000 0000 0000 0000 582f 0100 0000 0000  ........X/......
-00000bf0: 0204 0000 1800 0000 0000 0000 0000 0000  ................
-00000c00: 602f 0100 0000 0000 0204 0000 1900 0000  `/..............
-00000c10: 0000 0000 0000 0000 682f 0100 0000 0000  ........h/......
-00000c20: 0204 0000 1a00 0000 0000 0000 0000 0000  ................
-00000c30: 702f 0100 0000 0000 0204 0000 1b00 0000  p/..............
-00000c40: 0000 0000 0000 0000 782f 0100 0000 0000  ........x/......
-00000c50: 0204 0000 1c00 0000 0000 0000 0000 0000  ................
-00000c60: 802f 0100 0000 0000 0204 0000 1e00 0000  ./..............
-00000c70: 0000 0000 0000 0000 882f 0100 0000 0000  ........./......
-00000c80: 0204 0000 2000 0000 0000 0000 0000 0000  .... ...........
-00000c90: 902f 0100 0000 0000 0204 0000 2100 0000  ./..........!...
-00000ca0: 0000 0000 0000 0000 982f 0100 0000 0000  ........./......
-00000cb0: 0204 0000 2400 0000 0000 0000 0000 0000  ....$...........
-00000cc0: a02f 0100 0000 0000 0204 0000 2600 0000  ./..........&...
-00000cd0: 0000 0000 0000 0000 a82f 0100 0000 0000  ........./......
-00000ce0: 0204 0000 2700 0000 0000 0000 0000 0000  ....'...........
-00000cf0: b02f 0100 0000 0000 0204 0000 2800 0000  ./..........(...
-00000d00: 0000 0000 0000 0000 b82f 0100 0000 0000  ........./......
-00000d10: 0204 0000 2900 0000 0000 0000 0000 0000  ....)...........
-00000d20: c02f 0100 0000 0000 0204 0000 2e00 0000  ./..............
-00000d30: 0000 0000 0000 0000 c82f 0100 0000 0000  ........./......
-00000d40: 0204 0000 2f00 0000 0000 0000 0000 0000  ..../...........
-00000d50: d02f 0100 0000 0000 0204 0000 3200 0000  ./..........2...
-00000d60: 0000 0000 0000 0000 d82f 0100 0000 0000  ........./......
-00000d70: 0204 0000 3300 0000 0000 0000 0000 0000  ....3...........
-00000d80: e02f 0100 0000 0000 0204 0000 3400 0000  ./..........4...
-00000d90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000da0: f07b bfa9 9000 00d0 116e 47f9 1062 3b91  .{.......nG..b;.
-00000db0: 2002 1fd6 1f20 03d5 1f20 03d5 1f20 03d5   .... ... ... ..
-00000dc0: 9000 00d0 1172 47f9 1082 3b91 2002 1fd6  .....rG...;. ...
-00000dd0: 9000 00d0 1176 47f9 10a2 3b91 2002 1fd6  .....vG...;. ...
-00000de0: 9000 00d0 117a 47f9 10c2 3b91 2002 1fd6  .....zG...;. ...
-00000df0: 9000 00d0 117e 47f9 10e2 3b91 2002 1fd6  .....~G...;. ...
-00000e00: 9000 00d0 1182 47f9 1002 3c91 2002 1fd6  ......G...<. ...
-00000e10: 9000 00d0 1186 47f9 1022 3c91 2002 1fd6  ......G.."<. ...
-00000e20: 9000 00d0 118a 47f9 1042 3c91 2002 1fd6  ......G..B<. ...
-00000e30: 9000 00d0 118e 47f9 1062 3c91 2002 1fd6  ......G..b<. ...
-00000e40: 9000 00d0 1192 47f9 1082 3c91 2002 1fd6  ......G...<. ...
-00000e50: 9000 00d0 1196 47f9 10a2 3c91 2002 1fd6  ......G...<. ...
-00000e60: 9000 00d0 119a 47f9 10c2 3c91 2002 1fd6  ......G...<. ...
-00000e70: 9000 00d0 119e 47f9 10e2 3c91 2002 1fd6  ......G...<. ...
-00000e80: 9000 00d0 11a2 47f9 1002 3d91 2002 1fd6  ......G...=. ...
-00000e90: 9000 00d0 11a6 47f9 1022 3d91 2002 1fd6  ......G.."=. ...
-00000ea0: 9000 00d0 11aa 47f9 1042 3d91 2002 1fd6  ......G..B=. ...
-00000eb0: 9000 00d0 11ae 47f9 1062 3d91 2002 1fd6  ......G..b=. ...
-00000ec0: 9000 00d0 11b2 47f9 1082 3d91 2002 1fd6  ......G...=. ...
-00000ed0: 9000 00d0 11b6 47f9 10a2 3d91 2002 1fd6  ......G...=. ...
-00000ee0: 9000 00d0 11ba 47f9 10c2 3d91 2002 1fd6  ......G...=. ...
-00000ef0: 9000 00d0 11be 47f9 10e2 3d91 2002 1fd6  ......G...=. ...
-00000f00: 9000 00d0 11c2 47f9 1002 3e91 2002 1fd6  ......G...>. ...
-00000f10: 9000 00d0 11c6 47f9 1022 3e91 2002 1fd6  ......G..">. ...
-00000f20: 9000 00d0 11ca 47f9 1042 3e91 2002 1fd6  ......G..B>. ...
-00000f30: 9000 00d0 11ce 47f9 1062 3e91 2002 1fd6  ......G..b>. ...
-00000f40: 9000 00d0 11d2 47f9 1082 3e91 2002 1fd6  ......G...>. ...
-00000f50: 9000 00d0 11d6 47f9 10a2 3e91 2002 1fd6  ......G...>. ...
-00000f60: 9000 00d0 11da 47f9 10c2 3e91 2002 1fd6  ......G...>. ...
-00000f70: 9000 00d0 11de 47f9 10e2 3e91 2002 1fd6  ......G...>. ...
-00000f80: 9000 00d0 11e2 47f9 1002 3f91 2002 1fd6  ......G...?. ...
-00000f90: 9000 00d0 11e6 47f9 1022 3f91 2002 1fd6  ......G.."?. ...
-00000fa0: 9000 00d0 11ea 47f9 1042 3f91 2002 1fd6  ......G..B?. ...
-00000fb0: 9000 00d0 11ee 47f9 1062 3f91 2002 1fd6  ......G..b?. ...
-00000fc0: 9000 00d0 11f2 47f9 1082 3f91 2002 1fd6  ......G...?. ...
-00000fd0: 8000 00f0 0000 0091 8aff ff17 fd7b bfa9  .............{..
-00000fe0: fd03 0091 4000 00b4 0000 3fd6 fd7b c1a8  ....@.....?..{..
-00000ff0: c003 5fd6 e103 00aa 8200 00f0 0000 0090  .._.............
-00001000: 4200 0091 0070 3f91 b2ff ff17 ff83 01d1  B....p?.........
-00001010: 0200 0090 4280 3591 f55b 01a9 9500 00b0  ....B.5..[......
-00001020: f353 00a9 f763 02a9 a3fa 47f9 1300 0090  .S...c....G.....
-00001030: f97b 03a9 7342 3591 f403 00aa 6300 40f9  .{..sB5.....c.@.
-00001040: e103 13aa 8000 8052 e32f 00f9 7dff ff97  .......R./..}...
-00001050: 9802 40f9 e183 0191 0200 80d2 e003 18aa  ..@.............
-00001060: 220c 1ff8 0303 40f9 6310 40f9 6000 3fd6  ".....@.c.@.`.?.
-00001070: e32b 40f9 a316 00b4 0200 0090 e103 13aa  .+@.............
-00001080: 4200 3691 8000 8052 9742 0891 6dff ff97  B.6....R.B..m...
-00001090: e22b 40f9 0100 0090 2160 3691 e003 02aa  .+@.....!`6.....
-000010a0: 4200 40f9 4218 40f9 4000 3fd6 f603 00aa  B.@.B.@.@.?.....
-000010b0: e02b 40f9 0300 0090 0200 0090 e103 16aa  .+@.............
-000010c0: 6320 3791 42c0 3691 0400 40f9 84c4 41f9  c 7.B.6...@...A.
-000010d0: 8000 3fd6 e203 00aa e32b 40f9 e103 16aa  ..?......+@.....
-000010e0: e003 03aa 6300 40f9 63c8 41f9 6000 3fd6  ....c.@.c.A.`.?.
-000010f0: e027 00f9 e22b 40f9 8122 0091 e003 02aa  .'...+@.."......
-00001100: 4200 40f9 429c 42f9 4000 3fd6 f903 00aa  B.@.B.B.@.?.....
-00001110: e22b 40f9 8132 0491 e003 02aa 4200 40f9  .+@..2......B.@.
-00001120: 429c 42f9 4000 3fd6 e023 00f9 e22b 40f9  B.B.@.?..#...+@.
-00001130: 0100 0090 21a0 3791 e003 02aa 4200 40f9  ....!.7.....B.@.
-00001140: 4218 40f9 4000 3fd6 f603 00aa e02b 40f9  B.@.@.?......+@.
-00001150: 0200 0090 0300 0090 e103 16aa 4220 3891  ............B 8.
-00001160: 6340 3891 0700 40f9 e584 40f9 a000 3fd6  c@8...@...@...?.
-00001170: e203 00aa e02b 40f9 0500 80d2 e627 40f9  .....+@......'@.
-00001180: e103 16aa e423 40f9 e303 19aa 0800 40f9  .....#@.......@.
-00001190: 0771 40f9 e000 3fd6 e303 00aa 0200 0090  .q@...?.........
-000011a0: f903 00aa e103 13aa 42a0 3991 8000 8052  ........B.9....R
-000011b0: 24ff ff97 e02b 40f9 0200 0090 0300 0090  $....+@.........
-000011c0: 4200 3a91 e103 16aa 6340 3a91 0400 40f9  B.:.....c@:...@.
-000011d0: 8484 40f9 8000 3fd6 e023 00f9 e32b 40f9  ..@...?..#...+@.
-000011e0: e103 17aa e003 03aa 6300 40f9 639c 42f9  ........c.@.c.B.
-000011f0: 6000 3fd6 e303 00aa e42b 40f9 e103 19aa  `.?......+@.....
-00001200: e223 40f9 e003 04aa 8400 40f9 8488 40f9  .#@.......@...@.
-00001210: 8000 3fd6 f603 00aa 0200 0090 e103 13aa  ..?.............
-00001220: 42e0 3a91 8000 8052 e303 17aa e403 16aa  B.:....R........
-00001230: 04ff ff97 e22b 40f9 e003 02aa 4100 40f9  .....+@.....A.@.
-00001240: 213c 40f9 2000 3fd6 a003 00b4 e12b 40f9  !<@. .?......+@.
-00001250: e003 01aa 2100 40f9 2140 40f9 2000 3fd6  ....!.@.!@@. .?.
-00001260: e12b 40f9 e003 01aa 2100 40f9 2144 40f9  .+@.....!.@.!D@.
-00001270: 2000 3fd6 0200 0090 e103 13aa 4220 3b91   .?.........B ;.
-00001280: e303 17aa c000 8052 eefe ff97 b5fa 47f9  .......R......G.
-00001290: 0000 80d2 e22f 40f9 a102 40f9 5f00 01eb  ...../@...@._...
-000012a0: 0106 0054 f353 40a9 f55b 41a9 f763 42a9  ...T.S@..[A..cB.
-000012b0: f97b 43a9 ff83 0191 c003 5fd6 e42b 40f9  .{C......._..+@.
-000012c0: 8252 0c91 8362 1091 e103 16aa e003 04aa  .R...b..........
-000012d0: 8400 40f9 84c4 41f9 8000 3fd6 e023 00f9  ..@...A...?..#..
-000012e0: e32b 40f9 8172 1491 e003 03aa 6300 40f9  .+@..r......c.@.
-000012f0: 639c 42f9 6000 3fd6 e303 00aa e42b 40f9  c.B.`.?......+@.
-00001300: e103 16aa e223 40f9 e003 04aa 8400 40f9  .....#@.......@.
-00001310: 8434 42f9 8000 3fd6 0103 40f9 e003 18aa  .4B...?...@.....
-00001320: 2114 40f9 2000 3fd6 e003 14aa 25ff ff97  !.@. .?.....%...
-00001330: 0200 0090 e103 13aa 4280 3b91 8000 8052  ........B.;....R
-00001340: c0fe ff97 d2ff ff17 0200 0090 e103 13aa  ................
-00001350: 42c0 3591 c000 8052 bafe ff97 ccff ff17  B.5....R........
-00001360: c0fe ff97 ff03 0dd1 ff83 01d1 f55b 01a9  .............[..
-00001370: 9600 00b0 fe2b 00f9 f763 02a9 f96b 03a9  .....+...c...k..
-00001380: c8fa 47f9 f703 01aa f353 00a9 fb73 04a9  ..G......S...s..
-00001390: f903 03aa f803 05aa 0801 40f9 e503 02aa  ..........@.....
-000013a0: fa03 02aa 1500 0090 0200 0090 e303 00aa  ................
-000013b0: e603 19aa e703 18aa a142 3591 42c0 3b91  .........B5.B.;.
-000013c0: e437 00f9 fb03 00aa e403 17aa 8000 8052  .7.............R
-000013d0: e8cf 01f9 f403 0291 9afe ff97 8220 80d2  ............. ..
-000013e0: 0100 8052 e003 14aa cafe ff97 e003 14aa  ...R............
-000013f0: e103 17aa 8220 80d2 b2fe ff97 e803 14aa  ..... ..........
-00001400: 0901 4039 2911 0034 0805 00b1 a1ff ff54  ..@9)..4.......T
-00001410: 0800 8092 0001 4039 1fbc 0071 a100 0054  ......@9...q...T
-00001420: 0900 0014 0901 4039 3fbd 0071 c000 0054  ......@9?..q...T
-00001430: 0805 00f1 81ff ff54 0000 80d2 0000 0039  .......T.......9
-00001440: 007d 20d4 f303 08aa fc23 0691 8220 80d2  .} ......#... ..
-00001450: 0100 8052 e003 1caa 7f16 0038 adfe ff97  ...R.......8....
-00001460: e103 13aa 8220 80d2 e003 1caa 95fe ff97  ..... ..........
-00001470: 68fe ff97 e303 002a 0100 0090 e203 14aa  h......*........
-00001480: 2160 3c91 e003 14aa aefe ff97 0200 0090  !`<.............
-00001490: a142 3591 4280 3c91 e303 14aa 8000 8052  .B5.B.<........R
-000014a0: 68fe ff97 e003 14aa 0100 8052 b1fe ff97  h..........R....
-000014b0: 1f04 0031 c00d 0054 f343 0a91 0100 8052  ...1...T.C.....R
-000014c0: 8220 80d2 e003 13aa 92fe ff97 0100 0090  . ..............
-000014d0: e303 1caa 21e0 3c91 e203 14aa e003 13aa  ....!.<.........
-000014e0: 98fe ff97 e003 17aa 7700 0094 1c7c 4093  ........w....|@.
-000014f0: 3c0a 00b5 c901 0094 b542 3591 0200 0090  <........B5.....
-00001500: f303 00aa e303 00aa e103 15aa 4200 3d91  ............B.=.
-00001510: 8000 8052 fcc3 0191 4afe ff97 6202 40f9  ...R....J...b.@.
-00001520: e003 13aa e103 1caa 426c 43f9 4000 3fd6  ........BlC.@.?.
-00001530: f703 002a 400a 0035 8303 40f9 0200 0090  ...*@..5..@.....
-00001540: e103 15aa 42a0 3d91 8000 8052 3dfe ff97  ....B.=....R=...
-00001550: 00c4 80d2 33fe ff97 f303 00aa 8303 40f9  ....3.........@.
-00001560: e103 1baa 0384 00f8 8220 80d2 55fe ff97  ......... ..U...
-00001570: e103 14aa 8220 80d2 6032 0491 51fe ff97  ..... ..`2..Q...
-00001580: e103 1aaa 8220 80d2 6042 0891 4dfe ff97  ..... ..`B..M...
-00001590: e103 19aa 8220 80d2 6052 0c91 49fe ff97  ..... ..`R..I...
-000015a0: e137 40f9 8220 80d2 6062 1091 45fe ff97  .7@.. ..`b..E...
-000015b0: e103 18aa 8220 80d2 6072 1491 41fe ff97  ..... ..`r..A...
-000015c0: 0200 0090 e103 15aa 42e0 3d91 8000 8052  ........B.=....R
-000015d0: 1cfe ff97 8200 00b0 e0e3 0191 0100 80d2  ................
-000015e0: e303 13aa 42fc 47f9 f6fd ff97 e003 172a  ....B.G........*
-000015f0: d6fa 47f9 e2cf 41f9 c102 40f9 5f00 01eb  ..G...A...@._...
-00001600: e104 0054 f353 40a9 f55b 41a9 f763 42a9  ...T.S@..[A..cB.
-00001610: f96b 43a9 fb73 44a9 fe2b 40f9 ff83 0191  .kC..sD..+@.....
-00001620: ff03 0d91 c003 5fd6 0805 00f1 41ef ff54  ......_.....A..T
-00001630: 82ff ff17 e003 13aa 2300 0094 9fc3 20eb  ........#..... .
-00001640: a0f5 ff54 e003 14aa e13f 8052 09fe ff97  ...T.....?.R....
-00001650: e103 13aa e003 17aa 2e00 0094 e003 13aa  ................
-00001660: e13f 8052 03fe ff97 a3ff ff17 e003 14aa  .?.R............
-00001670: e13f 8052 4bfe ff97 90ff ff17 0200 0090  .?.RK...........
-00001680: c000 8052 e103 15aa 4240 3d91 e303 172a  ...R....B@=....*
-00001690: ecfd ff97 0000 8012 d6ff ff17 f1fd ff97  ................
-000016a0: 3cfe ff17 ff43 00d1 e003 022a fe03 00f9  <....C.....*....
-000016b0: f8fd ff97 0000 8052 fe03 40f9 ff43 0091  .......R..@..C..
-000016c0: c003 5fd6 ff83 02d1 e163 0091 f37b 00a9  .._......c...{..
-000016d0: 9300 00b0 73fa 47f9 6202 40f9 e24f 00f9  ....s.G.b.@..O..
-000016e0: 20fe ff97 1f00 1f6b e24f 40f9 e027 40f9   ......k.O@..'@.
-000016f0: 6102 40f9 00a0 9fda 5f00 01eb 8100 0054  a.@....._......T
-00001700: f37b 40a9 ff83 0291 c003 5fd6 d5fd ff97  .{@......._.....
-00001710: ffc3 00d1 0200 0090 e303 00aa 4240 3e91  ............B@>.
-00001720: f55b 01a9 1500 0090 f603 01aa b542 3591  .[...........B5.
-00001730: e403 16aa f353 00a9 e103 15aa f303 00aa  .....S..........
-00001740: 8000 8052 fe13 00f9 befd ff97 0100 0090  ...R............
-00001750: e003 13aa 2180 3e91 eafd ff97 f403 00aa  ....!.>.........
-00001760: 0003 00b4 0100 0090 e003 16aa 2100 3f91  ............!.?.
-00001770: e4fd ff97 f303 00aa 6000 00b5 1900 0014  ........`.......
-00001780: f4fd ff97 e003 14aa 9afd ff97 1f04 0031  ...............1
-00001790: e103 13aa 61ff ff54 e003 14aa e1fd ff97  ....a..T........
-000017a0: e003 13aa dffd ff97 0000 8052 f353 40a9  ...........R.S@.
-000017b0: f55b 41a9 fe13 40f9 ffc3 0091 c003 5fd6  .[A...@......._.
-000017c0: 0200 0090 c000 8052 e103 15aa 42a0 3e91  .......R....B.>.
-000017d0: e303 13aa 9bfd ff97 0000 8012 f4ff ff17  ................
-000017e0: 0200 0090 c000 8052 e103 15aa 42a0 3e91  .......R....B.>.
-000017f0: e303 16aa 93fd ff97 0000 8012 ecff ff17  ................
-00001800: ff43 10d1 0100 0090 ffc3 00d1 2160 3591  .C..........!`5.
-00001810: f55b 01a9 9600 00b0 fe13 00f9 f353 00a9  .[...........S..
-00001820: f503 00aa 0000 0090 c2fa 47f9 0020 3f91  ..........G.. ?.
-00001830: f3e3 0091 4200 40f9 e21f 02f9 b1fd ff97  ....B.@.........
-00001840: f403 00aa c000 00b5 2400 0014 e003 13aa  ........$.......
-00001850: e103 15aa 93fd ff97 a002 00b5 e003 13aa  ................
-00001860: 0180 8052 e203 14aa 5efd ff97 00ff ffb5  ...R....^.......
-00001870: 1300 80d2 e003 14aa aafd ff97 d6fa 47f9  ..............G.
-00001880: e003 13aa e21f 42f9 c102 40f9 5f00 01eb  ......B...@._...
-00001890: 8102 0054 f353 40a9 f55b 41a9 fe13 40f9  ...T.S@..[A...@.
-000018a0: ffc3 0091 ff43 1091 c003 5fd6 0100 0090  .....C...._.....
-000018b0: e003 13aa 2160 3f91 8afd ff97 0100 80d2  ....!`?.........
-000018c0: 0202 8052 5bfd ff97 1f20 40f1 f303 00aa  ...R[.... @.....
-000018d0: 21fd ff54 e7ff ff17 f303 00aa e8ff ff17  !..T............
-000018e0: 60fd ff97 ff83 03d1 f353 00a9 9400 00b0  `........S......
-000018f0: fe23 00f9 f55b 01a9 f763 02a9 82fa 47f9  .#...[...c....G.
-00001900: f603 01aa f96b 03a9 0100 8052 f503 00aa  .....k.....R....
-00001910: 4200 40f9 e26f 00f9 9afd ff97 1f04 0031  B.@..o.........1
-00001920: f703 002a e014 0054 e263 0191 e103 02aa  ...*...T.c......
-00001930: 5f7c 00a9 5f7c 01a9 5f7c 02a9 5f7c 03a9  _|.._|.._|.._|..
-00001940: 5f7c 04a9 5f7c 05a9 5f7c 06a9 5f7c 07a9  _|.._|.._|.._|..
-00001950: 4cfd ff97 f303 002a 600e 0035 1800 0090  L......*`..5....
-00001960: e48b 40b9 1a43 3591 0200 00b0 e303 15aa  ..@..C5.........
-00001970: e103 1aaa 4240 0091 6000 8052 f58b 80b9  ....B@..`..R....
-00001980: 30fd ff97 0000 80d2 e103 15aa 6200 8052  0...........b..R
-00001990: 4304 8052 e403 132a e503 00aa 2dfd ff97  C..R...*....-...
-000019a0: 1f04 00b1 f903 00aa 8012 0054 e103 132a  ...........T...*
-000019b0: e203 15aa 57fd ff97 e103 19aa e203 15aa  ....W...........
-000019c0: e003 172a 3bfd ff97 e003 172a 79fd ff97  ...*;......*y...
-000019d0: 2b77 4079 2717 40f9 ab0d 0034 e803 132a  +w@y'.@....4...*
-000019e0: 2703 078b f703 132a e503 132a e403 132a  '......*...*...*
-000019f0: e303 132a 0107 8052 0900 0014 df08 0071  ...*...R.......q
-00001a00: 6001 0054 df0c 0071 800b 0054 0805 0011  `..T...q...T....
-00001a10: e700 0191 1f01 0b6b 0004 0054 e604 40b9  .......k...T..@.
-00001a20: df2c 0071 e217 9f1a a2fe ff34 e610 40f9  .,.q.......4..@.
-00001a30: e41c 40f9 e318 40b9 c408 c49a 82fe ff34  ..@...@........4
-00001a40: 2a73 4079 2613 40f9 2afe ff34 c0e0 0091  *s@y&.@.*..4....
-00001a50: 4a05 0051 2603 068b 4a01 a19b 2a03 0a8b  J..Q&...J...*...
-00001a60: 0400 0014 c6e0 0091 df00 0aeb 00fd ff54  ...............T
-00001a70: c900 40b9 3f05 0071 61ff ff54 c204 40f9  ..@.?..qa..T..@.
-00001a80: 22ff ffb5 0805 0011 d710 40b9 1f01 0b6b  ".........@....k
-00001a90: e700 0191 41fc ff54 9f00 1f6b e117 9f1a  ....A..T...k....
-00001aa0: 7f00 1f6b e017 9f1a 2000 002a 6007 0035  ...k.... ..*`..5
-00001ab0: 4507 0034 9f00 1f6b 637c 4093 ba7c 4093  E..4...kc|@..|@.
-00001ac0: 2d09 0054 8404 0051 6060 0091 1803 8052  -..T...Q``.....R
-00001ad0: 3303 038b 9800 b89b 3803 188b 0400 0014  3.......8.......
-00001ae0: 7362 0091 7f02 18eb e007 0054 6202 40b9  sb.........Tb.@.
-00001af0: e103 16aa 4000 1a8b 2003 008b 0dfd ff97  ....@... .......
-00001b00: 00ff ff35 e003 19aa e103 15aa 7306 40f9  ...5........s.@.
-00001b10: b0fc ff97 7f02 1f6b 6002 174b 0010 931a  .......k`..K....
-00001b20: 0a00 0014 0100 0090 0200 0090 c000 8052  ...............R
-00001b30: 2140 3591 42e0 3f91 e303 15aa e403 132a  !@5.B.?........*
-00001b40: c0fc ff97 0000 8052 94fa 47f9 e26f 40f9  .......R..G..o@.
-00001b50: 8102 40f9 5f00 01eb e105 0054 f353 40a9  ..@._......T.S@.
-00001b60: f55b 41a9 f763 42a9 f96b 43a9 fe23 40f9  .[A..cB..kC..#@.
-00001b70: ff83 0391 c003 5fd6 207f 4079 1f00 086b  ......_. .@y...k
-00001b80: 60f4 ff54 e518 40b9 a1ff ff17 e303 0b2a  `..T..@........*
-00001b90: e403 0b2a e503 0b2a 0200 00b0 0143 3591  ...*...*.....C5.
-00001ba0: 42e0 0091 c000 8052 a6fc ff97 e003 19aa  B......R........
-00001bb0: e103 15aa 87fc ff97 0000 8052 e3ff ff17  ...........R....
-00001bc0: 0100 0090 0200 0090 c000 8052 2140 3591  ...........R!@5.
-00001bd0: 4280 3f91 e303 15aa 9afc ff97 0000 8052  B.?............R
-00001be0: daff ff17 e003 19aa e103 15aa 79fc ff97  ............y...
-00001bf0: 0000 8052 d5ff ff17 0200 00b0 c000 8052  ...R...........R
-00001c00: e103 1aaa 4280 0091 8efc ff97 e003 132a  ....B..........*
-00001c10: ceff ff17 93fc ff97 ff03 01d1 0000 80d2  ................
-00001c20: f353 00a9 1400 00b0 fe1b 00f9 94e2 0191  .S..............
-00001c30: e103 14aa f55b 01a9 f763 02a9 adfc ff97  .....[...c......
-00001c40: f303 00aa e001 00b4 0100 0090 0200 00b0  ................
-00001c50: e303 00aa 2140 3591 4280 0291 8000 8052  ....!@5.B......R
-00001c60: 78fc ff97 6002 3fd6 f353 40a9 f55b 41a9  x...`.?..S@..[A.
-00001c70: f763 42a9 fe1b 40f9 ff03 0191 c003 5fd6  .cB...@......._.
-00001c80: 1500 00b0 1700 0090 b5e2 0291 f742 3591  .............B5.
-00001c90: e003 15aa dbfe ff97 f803 00aa 0200 00b0  ................
-00001ca0: 8000 8052 e103 17aa 4280 0391 e303 15aa  ...R....B.......
-00001cb0: e403 18aa 63fc ff97 d803 00b4 e103 14aa  ....c...........
-00001cc0: e003 15aa 08ff ff97 f603 002a 0200 00b0  ...........*....
-00001cd0: 8000 8052 e103 17aa 4260 0491 e303 14aa  ...R....B`......
-00001ce0: e403 162a 57fc ff97 3601 0034 1643 368b  ...*W...6..4.C6.
-00001cf0: c002 3fd6 fe1b 40f9 f353 40a9 f55b 41a9  ..?...@..S@..[A.
-00001d00: f763 42a9 ff03 0191 c003 5fd6 0200 00b0  .cB......._.....
-00001d10: c000 8052 e103 17aa 42e0 0491 e303 14aa  ...R....B.......
-00001d20: e403 15aa 47fc ff97 e003 13aa cfff ff17  ....G...........
-00001d30: 0200 00b0 c000 8052 e103 17aa 42e0 0391  .......R....B...
-00001d40: 40fc ff97 e003 18aa c8ff ff17 0000 0000  @...............
-00001d50: 6465 786c 6f61 6465 7200 0000 0000 0000  dexloader.......
-00001d60: 456e 7465 7220 7468 7265 6164 0000 0000  Enter thread....
-00001d70: 4765 7420 656e 7620 6661 696c 6564 0000  Get env failed..
-00001d80: 4375 7272 656e 7420 4a4e 4945 6e76 3a20  Current JNIEnv: 
-00001d90: 2570 0000 0000 0000 6a61 7661 2f6c 616e  %p......java/lan
-00001da0: 672f 436c 6173 734c 6f61 6465 7200 0000  g/ClassLoader...
-00001db0: 6765 7453 7973 7465 6d43 6c61 7373 4c6f  getSystemClassLo
-00001dc0: 6164 6572 0000 0000 2829 4c6a 6176 612f  ader....()Ljava/
-00001dd0: 6c61 6e67 2f43 6c61 7373 4c6f 6164 6572  lang/ClassLoader
-00001de0: 3b00 0000 0000 0000 6461 6c76 696b 2f73  ;.......dalvik/s
-00001df0: 7973 7465 6d2f 4465 7843 6c61 7373 4c6f  ystem/DexClassLo
-00001e00: 6164 6572 0000 0000 3c69 6e69 743e 0000  ader....<init>..
-00001e10: 284c 6a61 7661 2f6c 616e 672f 5374 7269  (Ljava/lang/Stri
-00001e20: 6e67 3b4c 6a61 7661 2f6c 616e 672f 5374  ng;Ljava/lang/St
-00001e30: 7269 6e67 3b4c 6a61 7661 2f6c 616e 672f  ring;Ljava/lang/
-00001e40: 5374 7269 6e67 3b4c 6a61 7661 2f6c 616e  String;Ljava/lan
-00001e50: 672f 436c 6173 734c 6f61 6465 723b 2956  g/ClassLoader;)V
-00001e60: 0000 0000 0000 0000 4f62 6a65 6374 2064  ........Object d
-00001e70: 6578 5f6c 6f61 6465 723a 2025 7000 0000  ex_loader: %p...
-00001e80: 6669 6e64 436c 6173 7300 0000 0000 0000  findClass.......
-00001e90: 284c 6a61 7661 2f6c 616e 672f 5374 7269  (Ljava/lang/Stri
-00001ea0: 6e67 3b29 4c6a 6176 612f 6c61 6e67 2f43  ng;)Ljava/lang/C
-00001eb0: 6c61 7373 3b00 0000 436c 6173 7320 2573  lass;...Class %s
-00001ec0: 3a20 2570 0000 0000 4669 6e64 2063 6c61  : %p....Find cla
-00001ed0: 7373 2025 7320 6661 696c 6564 0000 0000  ss %s failed....
-00001ee0: 4578 6974 2074 6872 6561 6400 0000 0000  Exit thread.....
-00001ef0: 4c6f 6164 2064 6578 2025 7320 746f 2025  Load dex %s to %
-00001f00: 732c 2061 6e64 2063 616c 6c20 2573 2e25  s, and call %s.%
-00001f10: 7320 2573 0a00 0000 2573 2f25 6400 0000  s %s....%s/%d...
-00001f20: 4f75 7420 6669 6c65 2064 6972 3a20 2573  Out file dir: %s
-00001f30: 0000 0000 0000 0000 2573 2f25 7300 0000  ........%s/%s...
-00001f40: 4a4e 4945 6e76 3a20 2570 0a00 0000 0000  JNIEnv: %p......
-00001f50: 4765 7420 6a76 6d20 6661 696c 6564 3a20  Get jvm failed: 
-00001f60: 2564 0000 0000 0000 4a61 7661 564d 3a20  %d......JavaVM: 
-00001f70: 2570 0000 0000 0000 4372 6561 7465 206c  %p......Create l
-00001f80: 6f61 6469 6e67 2074 6872 6561 6400 0000  oading thread...
-00001f90: 636f 7079 2025 7320 746f 2025 730a 0000  copy %s to %s...
-00001fa0: 7262 0000 0000 0000 6f70 656e 2025 7320  rb......open %s 
-00001fb0: 6572 726f 7220 210a 0000 0000 0000 0000  error !.........
-00001fc0: 7762 0000 0000 0000 2f70 726f 632f 7365  wb....../proc/se
-00001fd0: 6c66 2f6d 6170 7300 2d00 0000 0000 0000  lf/maps.-.......
-00001fe0: 6361 6e6e 6f74 206f 7065 6e20 2725 7327  cannot open '%s'
-00001ff0: 0000 0000 0000 0000 6673 7461 7420 2573  ........fstat %s
-00002000: 2066 6169 6c65 643a 2025 6400 0000 0000   failed: %d.....
-00002010: 2573 2073 697a 653a 2025 6400 0000 0000  %s size: %d.....
-00002020: 416c 6c6f 6320 6d65 6d6f 7279 2066 6169  Alloc memory fai
-00002030: 6c65 6400 0000 0000 7379 6d74 6162 5f6f  led.....symtab_o
-00002040: 6666 7365 743d 3078 2578 2073 796d 7461  ffset=0x%x symta
-00002050: 625f 656e 7472 6965 733d 3078 2578 2073  b_entries=0x%x s
-00002060: 7472 7461 625f 6f66 6673 6574 3d30 7825  trtab_offset=0x%
-00002070: 7800 0000 0000 0000 5f5a 4e37 616e 6472  x......._ZN7andr
-00002080: 6f69 6431 3441 6e64 726f 6964 5275 6e74  oid14AndroidRunt
-00002090: 696d 6539 6765 744a 4e49 456e 7645 7600  ime9getJNIEnvEv.
-000020a0: 6765 744a 4e49 456e 7620 6279 2064 6c73  getJNIEnv by dls
-000020b0: 796d 3a20 2570 0000 2f73 7973 7465 6d2f  ym: %p../system/
-000020c0: 6c69 6236 342f 6c69 6261 6e64 726f 6964  lib64/libandroid
-000020d0: 5f72 756e 7469 6d65 2e73 6f00 0000 0000  _runtime.so.....
-000020e0: 4d6f 6475 6c65 2025 7320 6261 7365 3a20  Module %s base: 
-000020f0: 2570 0000 0000 0000 4d75 7374 2072 756e  %p......Must run
-00002100: 2069 6e20 416e 6472 6f69 6420 6170 7020   in Android app 
-00002110: 7072 6f63 6573 7300 4675 6e63 7469 6f6e  process.Function
-00002120: 2025 7320 6f66 6673 6574 3a20 3078 2578   %s offset: 0x%x
-00002130: 0000 0000 0000 0000 4675 6e63 7469 6f6e  ........Function
-00002140: 2025 7320 6e6f 7420 666f 756e 6420 696e   %s not found in
-00002150: 2025 7300 0000 0000 011b 033b 5400 0000   %s........;T...
-00002160: 0900 0000 b4ee ffff 7000 0000 0cf2 ffff  ........p.......
-00002170: b000 0000 48f5 ffff 0001 0000 4cf5 ffff  ....H.......L...
-00002180: 1801 0000 6cf5 ffff 3801 0000 b8f5 ffff  ....l...8.......
-00002190: 6001 0000 a8f6 ffff 9001 0000 8cf7 ffff  `...............
-000021a0: d001 0000 c0fa ffff 1002 0000 0000 0000  ................
-000021b0: 1400 0000 0000 0000 017a 5200 0478 1e01  .........zR..x..
-000021c0: 1b0c 1f00 0000 0000 3c00 0000 1c00 0000  ........<.......
-000021d0: 3cee ffff 5803 0000 0041 0e60 4395 0a96  <...X....A.`C...
-000021e0: 0944 930c 940b 9708 9807 4299 069e 0502  .D........B.....
-000021f0: 9d0a d4d3 41d6 d541 d8d7 41de d941 0e00  ....A..A..A..A..
-00002200: 410b 0000 0000 0000 4c00 0000 5c00 0000  A.......L...\...
-00002210: 54f1 ffff 3c03 0000 0041 0ec0 0641 0ea0  T...<....A...A..
-00002220: 0741 9572 9671 459e 6a97 7098 6f99 6e9a  .A.r.qE.j.p.o.n.
-00002230: 6d43 9374 9473 9b6c 9c6b 029e 0ad4 d341  mC.t.s.l.k.....A
-00002240: d6d5 41d8 d741 dad9 41dc db41 de41 0ec0  ..A..A..A..A.A..
-00002250: 0641 0ee0 0541 0b00 1400 0000 ac00 0000  .A...A..........
-00002260: 40f4 ffff 0400 0000 0000 0000 0000 0000  @...............
-00002270: 1c00 0000 c400 0000 2cf4 ffff 2000 0000  ........,... ...
-00002280: 0041 0e10 429e 0243 de41 0e00 0000 0000  .A..B..C.A......
-00002290: 2400 0000 e400 0000 2cf4 ffff 4c00 0000  $.......,...L...
-000022a0: 0041 0ea0 0142 9314 9e13 4d0a ded3 410e  .A...B....M...A.
-000022b0: 0041 0b00 0000 0000 2c00 0000 0c01 0000  .A......,.......
-000022c0: 50f4 ffff f000 0000 0041 0e30 4495 0496  P........A.0D...
-000022d0: 0346 9306 9405 439e 025a 0ad4 d341 d6d5  .F....C..Z...A..
-000022e0: 41de 410e 0041 0b00 3c00 0000 3c01 0000  A.A..A..<...<...
-000022f0: 10f5 ffff e400 0000 0041 0e90 0842 0ec0  .........A...B..
-00002300: 0842 9586 0196 8501 439e 8401 9388 0194  .B......C.......
-00002310: 8701 5e0a d4d3 41d6 d541 de41 0e90 0841  ..^...A..A.A...A
-00002320: 0ee0 0741 0b00 0000 3c00 0000 7c01 0000  ...A....<...|...
-00002330: b4f5 ffff 3403 0000 0041 0ee0 0141 931c  ....4....A...A..
-00002340: 941b 459e 1495 1a96 1997 1898 1742 9916  ..E..........B..
-00002350: 9a15 0296 0ad4 d341 d6d5 41d8 d741 dad9  .......A..A..A..
-00002360: 41de 410e 0041 0b00 4400 0000 bc01 0000  A.A..A..D.......
-00002370: a8f8 ffff 3401 0000 0041 0e40 4293 0894  ....4....A.@B...
-00002380: 0746 9e02 9506 9605 9704 9803 4c0a d4d3  .F..........L...
-00002390: 41d6 d541 d8d7 41de 410e 0041 0b5e 0ade  A..A..A.A..A.^..
-000023a0: 41d3 d441 d5d6 41d7 d841 0e00 410b 0000  A..A..A..A..A...
-000023b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000023c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000023d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000023e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000023f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002400: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002410: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002420: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002430: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002440: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002450: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002460: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002470: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002480: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002490: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000024a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000024b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000024c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000024d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000024e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000024f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002500: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002510: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002520: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002530: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002540: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002550: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002560: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002570: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002580: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002590: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000025a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000025b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000025c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000025d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000025e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000025f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002600: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002610: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002620: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002630: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002640: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002650: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002660: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002670: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002680: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002690: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000026a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000026b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000026c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000026d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000026e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000026f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002700: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002710: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002720: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002730: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002740: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002750: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002760: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002770: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002780: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002790: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000027a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000027b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000027c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000027d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000027e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000027f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002800: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002810: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002820: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002830: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002840: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002850: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002860: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002870: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002880: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002890: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000028a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000028b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000028c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000028d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000028e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000028f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002900: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002910: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002920: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002930: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002940: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002950: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002960: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002970: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002980: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002990: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000029a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000029b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000029c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000029d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000029e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000029f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002a00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002a10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002a20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002a30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002a40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002a50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002a60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000007e0: fa00 0000 1200 0a00 dc16 0000 0000 0000  ................
+000007f0: ec02 0000 0000 0000 dc01 0000 1200 0000  ................
+00000800: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000810: 3002 0000 1000 f1ff 0830 0100 0000 0000  0........0......
+00000820: 0000 0000 0000 0000 1601 0000 1200 0000  ................
+00000830: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000840: 5102 0000 1000 f1ff 0830 0100 0000 0000  Q........0......
+00000850: 0000 0000 0000 0000 1d01 0000 1200 0000  ................
+00000860: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000870: 9e01 0000 1200 0000 0000 0000 0000 0000  ................
+00000880: 0000 0000 0000 0000 6502 0000 1000 f1ff  ........e.......
+00000890: 0830 0100 0000 0000 0000 0000 0000 0000  .0..............
+000008a0: c400 0000 1200 0000 0000 0000 0000 0000  ................
+000008b0: 0000 0000 0000 0000 7001 0000 1200 0000  ........p.......
+000008c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000008d0: d700 0000 1200 0a00 4420 0000 0000 0000  ........D ......
+000008e0: 3001 0000 0000 0000 1000 0000 1200 0000  0...............
+000008f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000900: 005f 5f63 7861 5f66 696e 616c 697a 6500  .__cxa_finalize.
+00000910: 5f5f 6378 615f 6174 6578 6974 004a 4e49  __cxa_atexit.JNI
+00000920: 5f4f 6e4c 6f61 6400 4a61 7661 5f63 6f6d  _OnLoad.Java_com
+00000930: 5f74 6573 745f 616e 6472 6f69 6473 7079  _test_androidspy
+00000940: 5f48 656c 7065 7255 7469 6c5f 6e61 7469  _HelperUtil_nati
+00000950: 7665 5365 7473 6964 004a 6176 615f 636f  veSetsid.Java_co
+00000960: 6d5f 7465 7374 5f61 6e64 726f 6964 7370  m_test_androidsp
+00000970: 795f 4865 6c70 6572 5574 696c 5f6e 6174  y_HelperUtil_nat
+00000980: 6976 6555 6d61 736b 005f 5f61 6e64 726f  iveUmask.__andro
+00000990: 6964 5f6c 6f67 5f70 7269 6e74 005f 5f73  id_log_print.__s
+000009a0: 7461 636b 5f63 686b 5f66 6169 6c00 6163  tack_chk_fail.ac
+000009b0: 6365 7373 0063 686d 6f64 0063 6f70 7966  cess.chmod.copyf
+000009c0: 696c 6500 6672 6565 0067 6574 5f66 696c  ile.free.get_fil
+000009d0: 655f 7369 7a65 0067 6574 5f6a 6e69 5f65  e_size.get_jni_e
+000009e0: 6e76 0067 6574 5f73 646b 5f76 6572 7369  nv.get_sdk_versi
+000009f0: 6f6e 0067 6574 7569 6400 6c6f 6164 5f64  on.getuid.load_d
+00000a00: 6578 006c 6f61 645f 6465 785f 696e 5f74  ex.load_dex_in_t
+00000a10: 6872 6561 6400 6d61 6c6c 6f63 006d 656d  hread.malloc.mem
+00000a20: 7365 7400 6d6b 6469 7200 7074 6872 6561  set.mkdir.pthrea
+00000a30: 645f 6372 6561 7465 0073 6574 4170 6942  d_create.setApiB
+00000a40: 6c61 636b 6c69 7374 4578 656d 7074 696f  lacklistExemptio
+00000a50: 6e73 0073 6574 7369 6400 7370 7269 6e74  ns.setsid.sprint
+00000a60: 6600 7374 726e 6370 7900 756d 6173 6b00  f.strncpy.umask.
+00000a70: 5f5f 7379 7374 656d 5f70 726f 7065 7274  __system_propert
+00000a80: 795f 6765 7400 6174 6f69 0064 6c73 796d  y_get.atoi.dlsym
+00000a90: 0066 636c 6f73 6500 6667 6574 7300 666f  .fclose.fgets.fo
+00000aa0: 7065 6e00 6670 7574 6300 6673 7461 7400  pen.fputc.fstat.
+00000ab0: 6765 745f 6d6f 6475 6c65 5f62 6173 6500  get_module_base.
+00000ac0: 6765 745f 7379 6d62 6f6c 5f6f 6666 7365  get_symbol_offse
+00000ad0: 7400 6765 7463 006d 6d61 7000 6d75 6e6d  t.getc.mmap.munm
+00000ae0: 6170 0073 7472 636d 7000 7374 7273 7472  ap.strcmp.strstr
+00000af0: 0073 7472 746f 6b00 7374 7274 6f75 6c00  .strtok.strtoul.
+00000b00: 6c69 626c 6f67 2e73 6f00 6c69 6263 2e73  liblog.so.libc.s
+00000b10: 6f00 6c69 626d 2e73 6f00 6c69 6273 7464  o.libm.so.libstd
+00000b20: 632b 2b2e 736f 006c 6962 646c 2e73 6f00  c++.so.libdl.so.
+00000b30: 5f65 6461 7461 005f 5f62 7373 5f73 7461  _edata.__bss_sta
+00000b40: 7274 005f 5f62 7373 5f73 7461 7274 5f5f  rt.__bss_start__
+00000b50: 005f 5f62 7373 5f65 6e64 5f5f 005f 5f65  .__bss_end__.__e
+00000b60: 6e64 5f5f 005f 656e 6400 6c69 6264 6578  nd__._end.libdex
+00000b70: 6c6f 6164 6572 2e73 6f00 4c49 4243 0000  loader.so.LIBC..
+00000b80: 0000 0000 0000 0200 0200 0100 0200 0200  ................
+00000b90: 0200 0200 0200 0100 0200 0200 0200 0200  ................
+00000ba0: 0100 0100 0200 0200 0200 0200 0200 0200  ................
+00000bb0: 0100 0100 0100 0200 0300 0100 0000 0100  ................
+00000bc0: 0200 0200 0200 0100 0100 0100 0200 0200  ................
+00000bd0: 0200 0100 0200 0100 0200 0100 0200 0100  ................
+00000be0: 0200 0100 0200 0200 0100 0200 0200 0100  ................
+00000bf0: 0200 0000 0000 0000 0100 0100 2702 0000  ............'...
+00000c00: 1000 0000 2000 0000 630d 0500 0000 0300  .... ...c.......
+00000c10: 7a02 0000 0000 0000 0100 0100 0a02 0000  z...............
+00000c20: 1000 0000 0000 0000 630d 0500 0000 0200  ........c.......
+00000c30: 7a02 0000 0000 0000 682c 0100 0000 0000  z.......h,......
+00000c40: 0304 0000 0000 0000 2013 0000 0000 0000  ........ .......
+00000c50: f82f 0100 0000 0000 0104 0000 2900 0000  ./..........)...
+00000c60: 0000 0000 0000 0000 a02e 0100 0000 0000  ................
+00000c70: 0204 0000 0300 0000 0000 0000 0000 0000  ................
+00000c80: a82e 0100 0000 0000 0204 0000 0400 0000  ................
+00000c90: 0000 0000 0000 0000 b02e 0100 0000 0000  ................
+00000ca0: 0204 0000 0600 0000 0000 0000 0000 0000  ................
+00000cb0: b82e 0100 0000 0000 0204 0000 0700 0000  ................
+00000cc0: 0000 0000 0000 0000 c02e 0100 0000 0000  ................
+00000cd0: 0204 0000 0800 0000 0000 0000 0000 0000  ................
+00000ce0: c82e 0100 0000 0000 0204 0000 0900 0000  ................
+00000cf0: 0000 0000 0000 0000 d02e 0100 0000 0000  ................
+00000d00: 0204 0000 0a00 0000 0000 0000 0000 0000  ................
+00000d10: d82e 0100 0000 0000 0204 0000 0b00 0000  ................
+00000d20: 0000 0000 0000 0000 e02e 0100 0000 0000  ................
+00000d30: 0204 0000 0c00 0000 0000 0000 0000 0000  ................
+00000d40: e82e 0100 0000 0000 0204 0000 0d00 0000  ................
+00000d50: 0000 0000 0000 0000 f02e 0100 0000 0000  ................
+00000d60: 0204 0000 0e00 0000 0000 0000 0000 0000  ................
+00000d70: f82e 0100 0000 0000 0204 0000 0f00 0000  ................
+00000d80: 0000 0000 0000 0000 002f 0100 0000 0000  ........./......
+00000d90: 0204 0000 1000 0000 0000 0000 0000 0000  ................
+00000da0: 082f 0100 0000 0000 0204 0000 1200 0000  ./..............
+00000db0: 0000 0000 0000 0000 102f 0100 0000 0000  ........./......
+00000dc0: 0204 0000 1300 0000 0000 0000 0000 0000  ................
+00000dd0: 182f 0100 0000 0000 0204 0000 1400 0000  ./..............
+00000de0: 0000 0000 0000 0000 202f 0100 0000 0000  ........ /......
+00000df0: 0204 0000 1500 0000 0000 0000 0000 0000  ................
+00000e00: 282f 0100 0000 0000 0204 0000 1600 0000  (/..............
+00000e10: 0000 0000 0000 0000 302f 0100 0000 0000  ........0/......
+00000e20: 0204 0000 1700 0000 0000 0000 0000 0000  ................
+00000e30: 382f 0100 0000 0000 0204 0000 1800 0000  8/..............
+00000e40: 0000 0000 0000 0000 402f 0100 0000 0000  ........@/......
+00000e50: 0204 0000 1900 0000 0000 0000 0000 0000  ................
+00000e60: 482f 0100 0000 0000 0204 0000 1b00 0000  H/..............
+00000e70: 0000 0000 0000 0000 502f 0100 0000 0000  ........P/......
+00000e80: 0204 0000 1c00 0000 0000 0000 0000 0000  ................
+00000e90: 582f 0100 0000 0000 0204 0000 1e00 0000  X/..............
+00000ea0: 0000 0000 0000 0000 602f 0100 0000 0000  ........`/......
+00000eb0: 0204 0000 2000 0000 0000 0000 0000 0000  .... ...........
+00000ec0: 682f 0100 0000 0000 0204 0000 2100 0000  h/..........!...
+00000ed0: 0000 0000 0000 0000 702f 0100 0000 0000  ........p/......
+00000ee0: 0204 0000 2200 0000 0000 0000 0000 0000  ...."...........
+00000ef0: 782f 0100 0000 0000 0204 0000 2300 0000  x/..........#...
+00000f00: 0000 0000 0000 0000 802f 0100 0000 0000  ........./......
+00000f10: 0204 0000 2500 0000 0000 0000 0000 0000  ....%...........
+00000f20: 882f 0100 0000 0000 0204 0000 2600 0000  ./..........&...
+00000f30: 0000 0000 0000 0000 902f 0100 0000 0000  ........./......
+00000f40: 0204 0000 2700 0000 0000 0000 0000 0000  ....'...........
+00000f50: 982f 0100 0000 0000 0204 0000 2800 0000  ./..........(...
+00000f60: 0000 0000 0000 0000 a02f 0100 0000 0000  ........./......
+00000f70: 0204 0000 2a00 0000 0000 0000 0000 0000  ....*...........
+00000f80: a82f 0100 0000 0000 0204 0000 2c00 0000  ./..........,...
+00000f90: 0000 0000 0000 0000 b02f 0100 0000 0000  ........./......
+00000fa0: 0204 0000 2e00 0000 0000 0000 0000 0000  ................
+00000fb0: b82f 0100 0000 0000 0204 0000 3000 0000  ./..........0...
+00000fc0: 0000 0000 0000 0000 c02f 0100 0000 0000  ........./......
+00000fd0: 0204 0000 3200 0000 0000 0000 0000 0000  ....2...........
+00000fe0: c82f 0100 0000 0000 0204 0000 3300 0000  ./..........3...
+00000ff0: 0000 0000 0000 0000 d02f 0100 0000 0000  ........./......
+00001000: 0204 0000 3500 0000 0000 0000 0000 0000  ....5...........
+00001010: d82f 0100 0000 0000 0204 0000 3600 0000  ./..........6...
+00001020: 0000 0000 0000 0000 e02f 0100 0000 0000  ........./......
+00001030: 0204 0000 3700 0000 0000 0000 0000 0000  ....7...........
+00001040: e82f 0100 0000 0000 0204 0000 3800 0000  ./..........8...
+00001050: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001060: f07b bfa9 9000 00b0 114e 47f9 1062 3a91  .{.......NG..b:.
+00001070: 2002 1fd6 1f20 03d5 1f20 03d5 1f20 03d5   .... ... ... ..
+00001080: 9000 00b0 1152 47f9 1082 3a91 2002 1fd6  .....RG...:. ...
+00001090: 9000 00b0 1156 47f9 10a2 3a91 2002 1fd6  .....VG...:. ...
+000010a0: 9000 00b0 115a 47f9 10c2 3a91 2002 1fd6  .....ZG...:. ...
+000010b0: 9000 00b0 115e 47f9 10e2 3a91 2002 1fd6  .....^G...:. ...
+000010c0: 9000 00b0 1162 47f9 1002 3b91 2002 1fd6  .....bG...;. ...
+000010d0: 9000 00b0 1166 47f9 1022 3b91 2002 1fd6  .....fG..";. ...
+000010e0: 9000 00b0 116a 47f9 1042 3b91 2002 1fd6  .....jG..B;. ...
+000010f0: 9000 00b0 116e 47f9 1062 3b91 2002 1fd6  .....nG..b;. ...
+00001100: 9000 00b0 1172 47f9 1082 3b91 2002 1fd6  .....rG...;. ...
+00001110: 9000 00b0 1176 47f9 10a2 3b91 2002 1fd6  .....vG...;. ...
+00001120: 9000 00b0 117a 47f9 10c2 3b91 2002 1fd6  .....zG...;. ...
+00001130: 9000 00b0 117e 47f9 10e2 3b91 2002 1fd6  .....~G...;. ...
+00001140: 9000 00b0 1182 47f9 1002 3c91 2002 1fd6  ......G...<. ...
+00001150: 9000 00b0 1186 47f9 1022 3c91 2002 1fd6  ......G.."<. ...
+00001160: 9000 00b0 118a 47f9 1042 3c91 2002 1fd6  ......G..B<. ...
+00001170: 9000 00b0 118e 47f9 1062 3c91 2002 1fd6  ......G..b<. ...
+00001180: 9000 00b0 1192 47f9 1082 3c91 2002 1fd6  ......G...<. ...
+00001190: 9000 00b0 1196 47f9 10a2 3c91 2002 1fd6  ......G...<. ...
+000011a0: 9000 00b0 119a 47f9 10c2 3c91 2002 1fd6  ......G...<. ...
+000011b0: 9000 00b0 119e 47f9 10e2 3c91 2002 1fd6  ......G...<. ...
+000011c0: 9000 00b0 11a2 47f9 1002 3d91 2002 1fd6  ......G...=. ...
+000011d0: 9000 00b0 11a6 47f9 1022 3d91 2002 1fd6  ......G.."=. ...
+000011e0: 9000 00b0 11aa 47f9 1042 3d91 2002 1fd6  ......G..B=. ...
+000011f0: 9000 00b0 11ae 47f9 1062 3d91 2002 1fd6  ......G..b=. ...
+00001200: 9000 00b0 11b2 47f9 1082 3d91 2002 1fd6  ......G...=. ...
+00001210: 9000 00b0 11b6 47f9 10a2 3d91 2002 1fd6  ......G...=. ...
+00001220: 9000 00b0 11ba 47f9 10c2 3d91 2002 1fd6  ......G...=. ...
+00001230: 9000 00b0 11be 47f9 10e2 3d91 2002 1fd6  ......G...=. ...
+00001240: 9000 00b0 11c2 47f9 1002 3e91 2002 1fd6  ......G...>. ...
+00001250: 9000 00b0 11c6 47f9 1022 3e91 2002 1fd6  ......G..">. ...
+00001260: 9000 00b0 11ca 47f9 1042 3e91 2002 1fd6  ......G..B>. ...
+00001270: 9000 00b0 11ce 47f9 1062 3e91 2002 1fd6  ......G..b>. ...
+00001280: 9000 00b0 11d2 47f9 1082 3e91 2002 1fd6  ......G...>. ...
+00001290: 9000 00b0 11d6 47f9 10a2 3e91 2002 1fd6  ......G...>. ...
+000012a0: 9000 00b0 11da 47f9 10c2 3e91 2002 1fd6  ......G...>. ...
+000012b0: 9000 00b0 11de 47f9 10e2 3e91 2002 1fd6  ......G...>. ...
+000012c0: 9000 00b0 11e2 47f9 1002 3f91 2002 1fd6  ......G...?. ...
+000012d0: 9000 00b0 11e6 47f9 1022 3f91 2002 1fd6  ......G.."?. ...
+000012e0: 9000 00b0 11ea 47f9 1042 3f91 2002 1fd6  ......G..B?. ...
+000012f0: 9000 00b0 11ee 47f9 1062 3f91 2002 1fd6  ......G..b?. ...
+00001300: 9000 00b0 11f2 47f9 1082 3f91 2002 1fd6  ......G...?. ...
+00001310: 9000 00b0 11f6 47f9 10a2 3f91 2002 1fd6  ......G...?. ...
+00001320: 8000 00d0 0000 0091 66ff ff17 fd7b bfa9  ........f....{..
+00001330: fd03 0091 4000 00b4 0000 3fd6 fd7b c1a8  ....@.....?..{..
+00001340: c003 5fd6 e103 00aa 8200 00d0 0000 0090  .._.............
+00001350: 4200 0091 00b0 0c91 eeff ff17 ff83 01d1  B...............
+00001360: f90b 00f9 f85f 02a9 f657 03a9 f44f 04a9  ....._...W...O..
+00001370: fd7b 05a9 fd43 0191 59d0 3bd5 2817 40f9  .{...C..Y.;.(.@.
+00001380: 0100 00b0 0200 00b0 f303 00aa 2120 0d91  ............! ..
+00001390: 4248 0d91 e003 1e32 e807 00f9 95ff ff97  BH.....2........
+000013a0: 7402 40f9 ff03 00f9 e103 0091 e203 1faa  t.@.............
+000013b0: 8802 40f9 e003 14aa 0811 40f9 0001 3fd6  ..@.......@...?.
+000013c0: e303 40f9 6312 00b4 0100 00b0 0200 00b0  ..@.c...........
+000013d0: 2120 0d91 42b8 0d91 e003 1e32 85ff ff97  ! ..B......2....
+000013e0: 98ff ff97 1f78 0071 2b01 0054 0100 00b0  .....x.q+..T....
+000013f0: 0200 00b0 2120 0d91 4204 0e91 e003 1e32  ....! ..B......2
+00001400: 7cff ff97 e003 40f9 3aff ff97 e003 40f9  |.....@.:.....@.
+00001410: 0100 00b0 2180 0e91 0800 40f9 0819 40f9  ....!.....@...@.
+00001420: 0001 3fd6 e803 40f9 f503 00aa 0200 00b0  ..?...@.........
+00001430: 0300 00b0 0901 40f9 42d8 0e91 632c 0f91  ......@.B...c,..
+00001440: e003 08aa 29c5 41f9 e103 15aa 2001 3fd6  ....).A..... .?.
+00001450: e803 40f9 e203 00aa e103 15aa 0901 40f9  ..@...........@.
+00001460: e003 08aa 29c9 41f9 2001 3fd6 f503 00aa  ....).A. .?.....
+00001470: e003 40f9 6122 0091 0800 40f9 089d 42f9  ..@.a"....@...B.
+00001480: 0001 3fd6 f603 00aa e003 40f9 6132 0491  ..?.......@.a2..
+00001490: 0800 40f9 089d 42f9 0001 3fd6 e803 40f9  ..@...B...?...@.
+000014a0: 0100 00b0 f703 00aa 2194 0f91 0901 40f9  ........!.....@.
+000014b0: e003 08aa 2919 40f9 2001 3fd6 e803 40f9  ....).@. .?...@.
+000014c0: f803 00aa 0200 00b0 0300 00b0 0901 40f9  ..............@.
+000014d0: 4208 1091 6324 1091 e003 08aa 2985 40f9  B...c$......).@.
+000014e0: e103 18aa 2001 3fd6 e803 40f9 e203 00aa  .... .?...@.....
+000014f0: e103 18aa e303 16aa 0901 40f9 e003 08aa  ..........@.....
+00001500: e403 17aa e503 1faa 2971 40f9 e603 15aa  ........)q@.....
+00001510: 2001 3fd6 1700 00b0 f603 00aa f722 0d91   .?.........."..
+00001520: 0200 00b0 4268 1191 e003 1e32 e103 17aa  ....Bh.....2....
+00001530: e303 16aa 2fff ff97 e003 40f9 0200 00b0  ..../.....@.....
+00001540: 0300 00b0 42c0 1191 0800 40f9 63e8 1191  ....B.....@.c...
+00001550: e103 18aa 0885 40f9 0001 3fd6 f803 00aa  ......@...?.....
+00001560: e003 40f9 7542 0891 e103 15aa 0800 40f9  ..@.uB........@.
+00001570: 089d 42f9 0001 3fd6 e803 40f9 e303 00aa  ..B...?...@.....
+00001580: e103 16aa e203 18aa 0901 40f9 e003 08aa  ..........@.....
+00001590: 2989 40f9 2001 3fd6 f603 00aa 0200 00b0  ).@. .?.........
+000015a0: 4280 1291 e003 1e32 e103 17aa e303 15aa  B......2........
+000015b0: e403 16aa 0fff ff97 e003 40f9 0800 40f9  ..........@...@.
+000015c0: 083d 40f9 0001 3fd6 e803 40f9 0901 40f9  .=@...?...@...@.
+000015d0: c002 00b4 2941 40f9 e003 08aa 2001 3fd6  ....)A@..... .?.
+000015e0: e003 40f9 0800 40f9 0845 40f9 0001 3fd6  ..@...@..E@...?.
+000015f0: 0100 00b0 0200 00b0 2120 0d91 42b4 1291  ........! ..B...
+00001600: e007 1f32 e303 15aa fafe ff97 2700 0014  ...2........'...
+00001610: 0100 00b0 0200 00b0 2120 0d91 427c 0d91  ........! ..B|..
+00001620: e007 1f32 2000 0014 29c5 41f9 6252 0c91  ...2 ...).A.bR..
+00001630: 6362 1091 e003 08aa e103 16aa 2001 3fd6  cb.......... .?.
+00001640: f503 00aa e003 40f9 6172 1491 0800 40f9  ......@.ar....@.
+00001650: 089d 42f9 0001 3fd6 e803 40f9 e303 00aa  ..B...?...@.....
+00001660: e103 16aa e203 15aa 0901 40f9 e003 08aa  ..........@.....
+00001670: 2935 42f9 2001 3fd6 8802 40f9 e003 14aa  )5B. .?...@.....
+00001680: 0815 40f9 0001 3fd6 e003 13aa 15ff ff97  ..@...?.........
+00001690: 0100 00b0 0200 00b0 2120 0d91 4208 1391  ........! ..B...
+000016a0: e003 1e32 d3fe ff97 2817 40f9 e907 40f9  ...2....(.@...@.
+000016b0: 1f01 09eb 2101 0054 fd7b 45a9 f44f 44a9  ....!..T.{E..OD.
+000016c0: f657 43a9 f85f 42a9 f90b 40f9 e003 1faa  .WC.._B...@.....
+000016d0: ff83 0191 c003 5fd6 aafe ff97 fc0f 1af8  ......_.........
+000016e0: fa67 01a9 f85f 02a9 f657 03a9 f44f 04a9  .g..._...W...O..
+000016f0: fd7b 05a9 fd43 0191 ffc3 0cd1 5ad0 3bd5  .{...C......Z.;.
+00001700: 4817 40f9 f303 05aa f503 03aa f603 02aa  H.@.............
+00001710: f803 01aa f703 00aa 0100 00b0 0200 00b0  ................
+00001720: f403 04aa 2120 0d91 4238 1391 e003 1e32  ....! ..B8.....2
+00001730: e303 17aa e403 18aa e503 16aa e603 15aa  ................
+00001740: e703 13aa a883 1af8 aafe ff97 e093 0891  ................
+00001750: 8220 8052 e103 1f2a f993 0891 d9fe ff97  . .R...*........
+00001760: e093 0891 8220 8052 e103 18aa 99fe ff97  ..... .R........
+00001770: 2817 4038 e8ff ff35 28e3 5f38 3907 00d1  (.@8...5(._89...
+00001780: 1fbd 0071 a1ff ff54 e083 0491 8220 8052  ...q...T..... .R
+00001790: e103 1f2a 3ff3 1f38 cafe ff97 e083 0491  ...*?..8........
+000017a0: 8220 8052 e103 19aa 8afe ff97 a9fe ff97  . .R............
+000017b0: 0100 00b0 e303 002a 21d0 1391 e093 0891  .......*!.......
+000017c0: e293 0891 93fe ff97 0100 00b0 0200 00b0  ................
+000017d0: 2120 0d91 42e8 1391 e003 1e32 e393 0891  ! ..B......2....
+000017e0: 84fe ff97 e093 0891 e103 1f2a 59fe ff97  ...........*Y...
+000017f0: 1f04 0031 8100 0054 e093 0891 e123 0032  ...1...T.....#.2
+00001800: 34fe ff97 e073 0091 8220 8052 e103 1f2a  4....s... .R...*
+00001810: acfe ff97 0100 00b0 212c 1491 e073 0091  ........!,...s..
+00001820: e293 0891 e383 0491 7afe ff97 e003 18aa  ........z.......
+00001830: 44fe ff97 f903 002a d901 0034 e073 0091  D......*...4.s..
+00001840: 40fe ff97 3f03 006b 4001 0054 e093 0891  @...?..k@..T....
+00001850: e123 0032 33fe ff97 e173 0091 e003 18aa  .#.23....s......
+00001860: 54fe ff97 e073 0091 e123 0032 2dfe ff97  T....s...#.2-...
+00001870: a4fe ff97 f803 00aa 0100 00b0 0200 00b0  ................
+00001880: 2120 0d91 4244 1491 e003 1e32 e303 18aa  ! ..BD.....2....
+00001890: 58fe ff97 0803 40f9 e143 0091 e003 18aa  X.....@..C......
+000018a0: 086d 43f9 0001 3fd6 e803 002a 4801 0034  .mC...?....*H..4
+000018b0: 0100 00b0 0200 00b0 2120 0d91 4274 1491  ........! ..Bt..
+000018c0: e007 1f32 e303 082a 4afe ff97 0000 8012  ...2...*J.......
+000018d0: 3100 0014 e30b 40f9 1800 00b0 1823 0d91  1.....@......#..
+000018e0: 0200 00b0 42c0 1491 e003 1e32 e103 18aa  ....B......2....
+000018f0: 40fe ff97 00c4 8052 6efe ff97 e80b 40f9  @......Rn.....@.
+00001900: f903 00aa 8220 8052 e103 17aa 0884 00f8  ..... .R........
+00001910: 30fe ff97 2033 0491 e193 0891 8220 8052  0... 3....... .R
+00001920: 2cfe ff97 2043 0891 8220 8052 e103 16aa  ,... C... .R....
+00001930: 28fe ff97 2053 0c91 8220 8052 e103 15aa  (... S... .R....
+00001940: 24fe ff97 2063 1091 8220 8052 e103 14aa  $... c... .R....
+00001950: 20fe ff97 2073 1491 8220 8052 e103 13aa   ... s... .R....
+00001960: 1cfe ff97 0200 00b0 42ec 1491 e003 1e32  ........B......2
+00001970: e103 18aa 1ffe ff97 8200 00b0 42fc 47f9  ............B.G.
+00001980: e023 0091 e103 1faa e303 19aa c1fd ff97  .#..............
+00001990: e003 1f2a 4817 40f9 a983 5af8 1f01 09eb  ...*H.@...Z.....
+000019a0: 2101 0054 ffc3 0c91 fd7b 45a9 f44f 44a9  !..T.....{E..OD.
+000019b0: f657 43a9 f85f 42a9 fa67 41a9 fc07 46f8  .WC.._B..gA...F.
+000019c0: c003 5fd6 effd ff97 dafd ff17 fd7b bfa9  .._..........{..
+000019d0: fd03 0091 e003 022a b6fd ff97 e003 1f2a  .......*.......*
+000019e0: fd7b c1a8 c003 5fd6 ff03 01d1 f50b 00f9  .{...._.........
+000019f0: f44f 02a9 fd7b 03a9 fdc3 0091 55d0 3bd5  .O...{......U.;.
+00001a00: a816 40f9 0100 00b0 0200 00b0 f403 00aa  ..@.............
+00001a10: 9300 8052 2120 0d91 4244 1591 e003 1e32  ...R! ..BD.....2
+00001a20: e807 00f9 3300 a072 f2fd ff97 05fe ff97  ....3..r........
+00001a30: 1f78 0071 0b03 0054 ff03 00f9 8802 40f9  .x.q...T......@.
+00001a40: 8200 8052 e103 0091 2200 a072 0819 40f9  ...R...."..r..@.
+00001a50: e003 14aa 0001 3fd6 0100 00b0 2120 0d91  ......?.....! ..
+00001a60: e000 0034 0200 00b0 4270 1591 e007 1f32  ...4....Bp.....2
+00001a70: e0fd ff97 1300 8012 0700 0014 0200 00b0  ................
+00001a80: 4204 0e91 e003 1e32 dafd ff97 e003 40f9  B......2......@.
+00001a90: 98fd ff97 a816 40f9 e907 40f9 1f01 09eb  ......@...@.....
+00001aa0: e100 0054 e003 132a fd7b 43a9 f44f 42a9  ...T...*.{C..OB.
+00001ab0: f50b 40f9 ff03 0191 c003 5fd6 b1fd ff97  ..@......._.....
+00001ac0: ff03 01d1 f313 00f9 fd7b 03a9 fdc3 0091  .........{......
+00001ad0: 0800 00b0 53d0 3bd5 08c5 1591 6916 40f9  ....S.;.....i.@.
+00001ae0: 0001 c03d 0000 00b0 0004 1691 e103 0091  ...=............
+00001af0: e90f 00f9 e003 803d fefd ff97 e003 0091  .......=........
+00001b00: 60fd ff97 6816 40f9 e90f 40f9 1f01 09eb  `...h.@...@.....
+00001b10: a100 0054 fd7b 43a9 f313 40f9 ff03 0191  ...T.{C...@.....
+00001b20: c003 5fd6 97fd ff97 ffc3 02d1 f34b 00f9  .._..........K..
+00001b30: fd7b 0aa9 fd83 0291 53d0 3bd5 6816 40f9  .{......S.;.h.@.
+00001b40: e123 0091 a883 1ef8 d2fd ff97 e81f 40f9  .#............@.
+00001b50: 6916 40f9 aa83 5ef8 1f00 0071 00a1 9fda  i.@...^....q....
+00001b60: 3f01 0aeb a100 0054 fd7b 4aa9 f34b 40f9  ?......T.{J..K@.
+00001b70: ffc3 0291 c003 5fd6 82fd ff97 f50f 1df8  ......_.........
+00001b80: f44f 01a9 fd7b 02a9 fd83 0091 f503 01aa  .O...{..........
+00001b90: f403 00aa 0100 00b0 0200 00b0 2120 0d91  ............! ..
+00001ba0: 4258 1691 e003 1e32 e303 14aa e403 15aa  BX.....2........
+00001bb0: 90fd ff97 0100 00b0 2194 1691 e003 14aa  ........!.......
+00001bc0: c4fd ff97 f303 00aa 5303 00b4 0100 00b0  ........S.......
+00001bd0: 21e4 1691 e003 15aa befd ff97 f403 00aa  !...............
+00001be0: 5401 00b5 0100 00b0 0200 00b0 2120 0d91  T...........! ..
+00001bf0: 42a0 1691 e007 1f32 e303 15aa 1300 0014  B......2........
+00001c00: e103 14aa 5bfd ff97 e003 13aa 65fd ff97  ....[.......e...
+00001c10: 1f04 0031 61ff ff54 e003 13aa 51fd ff97  ...1a..T....Q...
+00001c20: e003 14aa 4ffd ff97 e003 1f2a 0900 0014  ....O......*....
+00001c30: 0100 00b0 0200 00b0 2120 0d91 42a0 1691  ........! ..B...
+00001c40: e007 1f32 e303 14aa 6afd ff97 0000 8012  ...2....j.......
+00001c50: fd7b 42a9 f44f 41a9 f507 43f8 c003 5fd6  .{B..OA...C..._.
+00001c60: fc57 bda9 f44f 01a9 fd7b 02a9 fd83 0091  .W...O...{......
+00001c70: ff43 10d1 55d0 3bd5 a816 40f9 f403 00aa  .C..U.;...@.....
+00001c80: 0000 00b0 0100 00b0 00f0 1691 21d0 0e91  ............!...
+00001c90: a883 1df8 8ffd ff97 f303 00aa 9302 00b4  ................
+00001ca0: e023 0091 e103 1632 e203 13aa 39fd ff97  .#.....2....9...
+00001cb0: 2002 00b4 e023 0091 e103 14aa 69fd ff97   ....#......i...
+00001cc0: 00ff ffb4 0100 00b0 2130 1791 e023 0091  ........!0...#..
+00001cd0: 68fd ff97 e203 1c32 e103 1faa 09fd ff97  h......2........
+00001ce0: 1f20 40f1 f403 809a 0400 0014 f403 1faa  . @.............
+00001cf0: 0400 0014 f403 1faa e003 13aa 19fd ff97  ................
+00001d00: a816 40f9 a983 5df8 1f01 09eb e100 0054  ..@...]........T
+00001d10: e003 14aa ff43 1091 fd7b 42a9 f44f 41a9  .....C...{B..OA.
+00001d20: fc57 c3a8 c003 5fd6 16fd ff97 ffc3 03d1  .W...._.........
+00001d30: fb4b 00f9 fa67 0aa9 f85f 0ba9 f657 0ca9  .K...g..._...W..
+00001d40: f44f 0da9 fd7b 0ea9 fd83 0391 58d0 3bd5  .O...{......X.;.
+00001d50: 0817 40f9 f403 01aa e103 1f2a f303 00aa  ..@........*....
+00001d60: a883 1af8 cffc ff97 f603 002a df06 0031  ...........*...1
+00001d70: 8002 0054 e023 0091 e203 1932 e103 1f2a  ...T.#.....2...*
+00001d80: 50fd ff97 e123 0091 e003 162a e1fc ff97  P....#.....*....
+00001d90: e803 002a 8802 0034 0100 00b0 0200 00b0  ...*...4........
+00001da0: 2120 0d91 427c 1791 e007 1f32 e303 13aa  ! ..B|.....2....
+00001db0: e403 082a 0ffd ff97 e003 1f2a 9500 0014  ...*.......*....
+00001dc0: 0100 00b0 0200 00b0 2120 0d91 4238 1791  ........! ..B8..
+00001dd0: e007 1f32 e303 13aa 06fd ff97 e003 1f2a  ...2...........*
+00001de0: 8c00 0014 f71f 40f9 0100 00b0 0200 00b0  ......@.........
+00001df0: 2120 0d91 42cc 1791 e007 0032 e303 13aa  ! ..B......2....
+00001e00: e403 172a fbfc ff97 f37e 4093 e207 0032  ...*.....~@....2
+00001e10: 4304 8052 e003 1faa e103 13aa e403 1f2a  C..R...........*
+00001e20: e503 1faa fffc ff97 f503 00aa bf06 00b1  ................
+00001e30: 600b 0054 e003 15aa e103 1f2a e203 13aa  `..T.......*....
+00001e40: 20fd ff97 e003 162a e103 15aa e203 172a   ......*.......*
+00001e50: a4fc ff97 e003 162a 0afd ff97 a876 4079  .......*.....v@y
+00001e60: e80a 00b4 aa16 40f9 e903 1faa e303 1f2a  ......@........*
+00001e70: f603 1f2a e503 1f2a e403 1f2a aa02 0a8b  ...*...*...*....
+00001e80: ab42 0091 4d19 098b ac05 40b9 9f2d 0071  .B..M.....@..-.q
+00001e90: a000 0054 9f0d 0071 0003 0054 9f09 0071  ...T...q...T...q
+00001ea0: a103 0054 ae11 40f9 af1d 40f9 a319 40b9  ...T..@...@...@.
+00001eb0: 9f2d 0071 c409 cf9a e102 0054 ac72 4079  .-.q.......T.r@y
+00001ec0: ac02 00b4 ae12 40f9 ed03 1faa 6e01 0e8b  ......@.....n...
+00001ed0: cf01 5fb8 ff05 0071 6100 0054 cf81 5ff8  .._....qa..T.._.
+00001ee0: 8f01 00b4 ad05 0091 bf01 0ceb cee1 0091  ................
+00001ef0: 0bff ff54 0800 0014 ac7e 4079 3f01 0ceb  ...T.....~@y?...
+00001f00: a000 0054 4c19 098b 8519 40b9 0200 0014  ...TL.....@.....
+00001f10: d601 40b9 7f00 0071 ecd7 9f1a 9f00 0071  ..@....q.......q
+00001f20: 2905 0091 edd7 9f1a bf00 0071 eed7 9f1a  )..........q....
+00001f30: 3f01 08eb 8a00 0054 ac01 0c0a cc01 0c0a  ?......T........
+00001f40: 2cfa ff34 2504 0034 0404 0034 e303 0034  ,..4%..4...4...4
+00001f50: 9f04 0071 0b02 0054 687c 4093 a802 088b  ...q...Th|@.....
+00001f60: f703 1faa b9c2 258b 9a7c 4093 1b21 0091  ......%..|@..!..
+00001f70: 6883 5fb8 e103 14aa 2003 088b a1fc ff97  h._..... .......
+00001f80: a003 0034 f706 0091 ff02 1aeb 7b63 0091  ...4........{c..
+00001f90: 0bff ff54 f403 1f2a 1800 0014 0100 00b0  ...T...*........
+00001fa0: 0200 00b0 2120 0d91 42fc 1791 e007 1f32  ....! ..B......2
+00001fb0: 90fc ff97 e003 1f2a 1600 0014 e303 1f2a  .......*.......*
+00001fc0: e503 1f2a e403 1f2a 0100 00b0 0200 00b0  ...*...*........
+00001fd0: 2120 0d91 424c 1891 e007 1f32 85fc ff97  ! ..BL.....2....
+00001fe0: e003 15aa e103 13aa aefc ff97 e003 1f2a  ...............*
+00001ff0: 0800 0014 7403 40b9 e003 15aa e103 13aa  ....t.@.........
+00002000: a8fc ff97 8802 164b 9f02 0071 e003 881a  .......K...q....
+00002010: 0817 40f9 a983 5af8 1f01 09eb 2101 0054  ..@...Z.....!..T
+00002020: fd7b 4ea9 f44f 4da9 f657 4ca9 f85f 4ba9  .{N..OM..WL.._K.
+00002030: fa67 4aa9 fb4b 40f9 ffc3 0391 c003 5fd6  .gJ..K@......._.
+00002040: 50fc ff97 f50f 1df8 f44f 01a9 fd7b 02a9  P........O...{..
+00002050: fd83 0091 0100 0090 2134 1991 e003 1faa  ........!4......
+00002060: 60fc ff97 e303 00aa a301 00b4 0100 0090  `...............
+00002070: 0200 0090 2120 0d91 42d4 1991 e003 1e32  ....! ..B......2
+00002080: e307 00f9 5bfc ff97 e007 40f9 fd7b 42a9  ....[.....@..{B.
+00002090: f44f 41a9 f507 43f8 0000 1fd6 1400 0090  .OA...C.........
+000020a0: 94a6 1f91 e003 14aa 46fc ff97 f303 00aa  ........F.......
+000020b0: 0100 0090 0200 0090 2120 0d91 4230 1a91  ........! ..B0..
+000020c0: e003 1e32 e303 14aa e403 13aa 49fc ff97  ...2........I...
+000020d0: 7302 00b4 1500 0090 0000 0090 b536 1991  s............6..
+000020e0: 00a4 1f91 e103 15aa 52fc ff97 f403 002a  ........R......*
+000020f0: 0100 0090 0200 0090 2120 0d91 42fc 1a91  ........! ..B...
+00002100: e003 1e32 e303 15aa e403 142a 39fc ff97  ...2.......*9...
+00002110: 5401 0034 6042 348b ddff ff17 0100 0090  T..4`B4.........
+00002120: 0200 0090 2120 0d91 427c 1a91 e007 1f32  ....! ..B|.....2
+00002130: 30fc ff97 0b00 0014 0100 0090 0200 0090  0...............
+00002140: 0300 0090 0400 0090 2120 0d91 4260 1b91  ........! ..B`..
+00002150: 6334 1991 84a4 1f91 e007 1f32 25fc ff97  c4.........2%...
+00002160: fd7b 42a9 f44f 41a9 e003 1faa f507 43f8  .{B..OA.......C.
+00002170: c003 5fd6 f85f bca9 f657 01a9 f44f 02a9  .._.._...W...O..
+00002180: fd7b 03a9 fdc3 0091 f303 00aa 6802 40f9  .{..........h.@.
+00002190: 0100 0090 21d0 1b91 0819 40f9 0001 3fd6  ....!.....@...?.
+000021a0: f403 00aa 340a 00b4 6802 40f9 0200 0090  ....4...h.@.....
+000021b0: 0300 0090 4218 0e91 08c5 41f9 63f4 1c91  ....B.....A.c...
+000021c0: e003 13aa e103 14aa 0001 3fd6 f503 00aa  ..........?.....
+000021d0: 1502 00b5 6802 40f9 e003 13aa 0845 40f9  ....h.@......E@.
+000021e0: 0001 3fd6 6802 40f9 0200 0090 0300 0090  ..?.h.@.........
+000021f0: 4250 1d91 08c5 41f9 63f4 1c91 e003 13aa  BP....A.c.......
+00002200: e103 14aa 0001 3fd6 f503 00aa 5508 00b4  ......?.....U...
+00002210: 6802 40f9 0100 0090 21d0 1e91 e003 13aa  h.@.....!.......
+00002220: 0819 40f9 0001 3fd6 6802 40f9 0100 0090  ..@...?.h.@.....
+00002230: f703 00aa 2114 1f91 089d 42f9 e003 13aa  ....!.....B.....
+00002240: 0001 3fd6 6802 40f9 f803 00aa e103 0032  ..?.h.@........2
+00002250: e003 13aa 08b1 42f9 e203 17aa e303 1faa  ......B.........
+00002260: f603 0032 0001 3fd6 6802 40f9 f703 00aa  ...2..?.h.@.....
+00002270: e003 13aa e103 17aa 08b9 42f9 e203 1f2a  ..........B....*
+00002280: e303 18aa 0001 3fd6 6802 40f9 e003 13aa  ......?.h.@.....
+00002290: e103 14aa e203 15aa 0835 42f9 e303 17aa  .........5B.....
+000022a0: 0001 3fd6 6802 40f9 e003 13aa e103 18aa  ..?.h.@.........
+000022b0: 085d 40f9 0001 3fd6 6802 40f9 e003 13aa  .]@...?.h.@.....
+000022c0: e103 17aa 085d 40f9 0001 3fd6 0100 0090  .....]@...?.....
+000022d0: 0200 0090 2120 0d91 421c 1f91 e003 1e32  ....! ..B......2
+000022e0: c4fb ff97 1300 0014 0100 0090 0200 0090  ................
+000022f0: 2120 0d91 425c 1c91 e007 1f32 bdfb ff97  ! ..B\.....2....
+00002300: 6802 40f9 e003 13aa 0845 40f9 0001 3fd6  h.@......E@...?.
+00002310: 0700 0014 0100 0090 0200 0090 2120 0d91  ............! ..
+00002320: 42b4 1d91 e007 1f32 b2fb ff97 f603 1f2a  B......2.......*
+00002330: e003 162a fd7b 43a9 f44f 42a9 f657 41a9  ...*.{C..OB..WA.
+00002340: f85f c4a8 c003 5fd6 6465 786c 6f61 6465  ._...._.dexloade
+00002350: 7200 456e 7465 7220 7468 7265 6164 0047  r.Enter thread.G
+00002360: 6574 2065 6e76 2066 6169 6c65 6400 4375  et env failed.Cu
+00002370: 7272 656e 7420 4a4e 4945 6e76 3a20 2570  rrent JNIEnv: %p
+00002380: 0043 616c 6c20 7365 7441 7069 426c 6163  .Call setApiBlac
+00002390: 6b6c 6973 7445 7865 6d70 7469 6f6e 7300  klistExemptions.
+000023a0: 6a61 7661 2f6c 616e 672f 436c 6173 734c  java/lang/ClassL
+000023b0: 6f61 6465 7200 6765 7453 7973 7465 6d43  oader.getSystemC
+000023c0: 6c61 7373 4c6f 6164 6572 0028 294c 6a61  lassLoader.()Lja
+000023d0: 7661 2f6c 616e 672f 436c 6173 734c 6f61  va/lang/ClassLoa
+000023e0: 6465 723b 0064 616c 7669 6b2f 7379 7374  der;.dalvik/syst
+000023f0: 656d 2f44 6578 436c 6173 734c 6f61 6465  em/DexClassLoade
+00002400: 7200 3c69 6e69 743e 0028 4c6a 6176 612f  r.<init>.(Ljava/
+00002410: 6c61 6e67 2f53 7472 696e 673b 4c6a 6176  lang/String;Ljav
+00002420: 612f 6c61 6e67 2f53 7472 696e 673b 4c6a  a/lang/String;Lj
+00002430: 6176 612f 6c61 6e67 2f53 7472 696e 673b  ava/lang/String;
+00002440: 4c6a 6176 612f 6c61 6e67 2f43 6c61 7373  Ljava/lang/Class
+00002450: 4c6f 6164 6572 3b29 5600 4f62 6a65 6374  Loader;)V.Object
+00002460: 2064 6578 5f6c 6f61 6465 723a 2025 7000   dex_loader: %p.
+00002470: 6669 6e64 436c 6173 7300 284c 6a61 7661  findClass.(Ljava
+00002480: 2f6c 616e 672f 5374 7269 6e67 3b29 4c6a  /lang/String;)Lj
+00002490: 6176 612f 6c61 6e67 2f43 6c61 7373 3b00  ava/lang/Class;.
+000024a0: 436c 6173 7320 2573 3a20 2570 0046 696e  Class %s: %p.Fin
+000024b0: 6420 636c 6173 7320 2573 2066 6169 6c65  d class %s faile
+000024c0: 6400 4578 6974 2074 6872 6561 6400 4c6f  d.Exit thread.Lo
+000024d0: 6164 2064 6578 2025 7320 746f 2025 732c  ad dex %s to %s,
+000024e0: 2061 6e64 2063 616c 6c20 2573 2e25 7320   and call %s.%s 
+000024f0: 2573 0a00 2573 2f25 6400 4f75 7420 6669  %s..%s/%d.Out fi
+00002500: 6c65 2064 6972 3a20 2573 0025 732f 2573  le dir: %s.%s/%s
+00002510: 004a 4e49 456e 763a 2025 700a 0047 6574  .JNIEnv: %p..Get
+00002520: 206a 766d 2066 6169 6c65 643a 2025 6400   jvm failed: %d.
+00002530: 4a61 7661 564d 3a20 2570 0043 7265 6174  JavaVM: %p.Creat
+00002540: 6520 6c6f 6164 696e 6720 7468 7265 6164  e loading thread
+00002550: 004a 4e49 5f4f 6e4c 6f61 6400 4552 524f  .JNI_OnLoad.ERRO
+00002560: 523a 2047 6574 456e 7620 6661 696c 6564  R: GetEnv failed
+00002570: 0030 0000 0000 0000 0000 0000 0000 0000  .0..............
+00002580: 0072 6f2e 6275 696c 642e 7665 7273 696f  .ro.build.versio
+00002590: 6e2e 7364 6b00 636f 7079 2025 7320 746f  n.sdk.copy %s to
+000025a0: 2025 730a 0072 6200 6f70 656e 2025 7320   %s..rb.open %s 
+000025b0: 6572 726f 7220 210a 0077 6200 2f70 726f  error !..wb./pro
+000025c0: 632f 7365 6c66 2f6d 6170 7300 2d00 6361  c/self/maps.-.ca
+000025d0: 6e6e 6f74 206f 7065 6e20 2725 7327 0066  nnot open '%s'.f
+000025e0: 7374 6174 2025 7320 6661 696c 6564 3a20  stat %s failed: 
+000025f0: 2564 0025 7320 7369 7a65 3a20 2564 0041  %d.%s size: %d.A
+00002600: 6c6c 6f63 206d 656d 6f72 7920 6661 696c  lloc memory fail
+00002610: 6564 0073 796d 7461 625f 6f66 6673 6574  ed.symtab_offset
+00002620: 3d30 7825 7820 7379 6d74 6162 5f65 6e74  =0x%x symtab_ent
+00002630: 7269 6573 3d30 7825 7820 7374 7274 6162  ries=0x%x strtab
+00002640: 5f6f 6666 7365 743d 3078 2578 005f 5a4e  _offset=0x%x._ZN
+00002650: 3761 6e64 726f 6964 3134 416e 6472 6f69  7android14Androi
+00002660: 6452 756e 7469 6d65 3967 6574 4a4e 4945  dRuntime9getJNIE
+00002670: 6e76 4576 0067 6574 4a4e 4945 6e76 2062  nvEv.getJNIEnv b
+00002680: 7920 646c 7379 6d3a 2025 7000 4d6f 6475  y dlsym: %p.Modu
+00002690: 6c65 2025 7320 6261 7365 3a20 2570 004d  le %s base: %p.M
+000026a0: 7573 7420 7275 6e20 696e 2041 6e64 726f  ust run in Andro
+000026b0: 6964 2061 7070 2070 726f 6365 7373 0046  id app process.F
+000026c0: 756e 6374 696f 6e20 2573 206f 6666 7365  unction %s offse
+000026d0: 743a 2030 7825 7800 4675 6e63 7469 6f6e  t: 0x%x.Function
+000026e0: 2025 7320 6e6f 7420 666f 756e 6420 696e   %s not found in
+000026f0: 2025 7300 636f 6d2f 616e 6472 6f69 642f   %s.com/android/
+00002700: 696e 7465 726e 616c 2f6f 732f 5a79 676f  internal/os/Zygo
+00002710: 7465 496e 6974 0043 6c61 7373 2061 6e64  teInit.Class and
+00002720: 726f 6964 2e6f 732e 5a79 676f 7465 496e  roid.os.ZygoteIn
+00002730: 6974 206e 6f74 2066 6f75 6e64 0028 5b4c  it not found.([L
+00002740: 6a61 7661 2f6c 616e 672f 5374 7269 6e67  java/lang/String
+00002750: 3b29 5600 7365 7441 7069 4465 6e79 6c69  ;)V.setApiDenyli
+00002760: 7374 4578 656d 7074 696f 6e73 004d 6574  stExemptions.Met
+00002770: 686f 6420 7365 7441 7069 426c 6163 6b6c  hod setApiBlackl
+00002780: 6973 7445 7865 6d70 7469 6f6e 7320 6f72  istExemptions or
+00002790: 2073 6574 4170 6944 656e 796c 6973 7445   setApiDenylistE
+000027a0: 7865 6d70 7469 6f6e 7320 6e6f 7420 666f  xemptions not fo
+000027b0: 756e 6400 6a61 7661 2f6c 616e 672f 5374  und.java/lang/St
+000027c0: 7269 6e67 004c 0073 6574 4170 6942 6c61  ring.L.setApiBla
+000027d0: 636b 6c69 7374 4578 656d 7074 696f 6e73  cklistExemptions
+000027e0: 2073 7563 6365 7373 002f 7379 7374 656d   success./system
+000027f0: 2f6c 6962 3634 2f6c 6962 616e 6472 6f69  /lib64/libandroi
+00002800: 645f 7275 6e74 696d 652e 736f 0000 0000  d_runtime.so....
+00002810: 011b 033b 6c00 0000 0c00 0000 4ceb ffff  ...;l.......L...
+00002820: 8800 0000 ccee ffff b000 0000 b8f1 ffff  ................
+00002830: e000 0000 bcf1 ffff f800 0000 d8f1 ffff  ................
+00002840: 1801 0000 b0f2 ffff 3801 0000 18f3 ffff  ........8.......
+00002850: 5801 0000 6cf3 ffff 7801 0000 50f4 ffff  X...l...x...P...
+00002860: 9801 0000 1cf5 ffff c001 0000 34f8 ffff  ............4...
+00002870: f001 0000 64f9 ffff 1002 0000 0000 0000  ....d...........
+00002880: 1400 0000 0000 0000 017a 5200 017c 1e01  .........zR..|..
+00002890: 1b0c 1f00 0000 0000 2400 0000 1c00 0000  ........$.......
+000028a0: bcea ffff 8003 0000 005c 0c1d 109e 029d  .........\......
+000028b0: 0493 0694 0895 0a96 0c97 0e98 1099 1400  ................
+000028c0: 2c00 0000 4400 0000 14ee ffff ec02 0000  ,...D...........
+000028d0: 0060 0c1d 109e 029d 0493 0694 0895 0a96  .`..............
+000028e0: 0c97 0e98 1099 129a 149c 1800 0000 0000  ................
+000028f0: 1400 0000 7400 0000 d0f0 ffff 0400 0000  ....t...........
+00002900: 0000 0000 0000 0000 1c00 0000 8c00 0000  ................
+00002910: bcf0 ffff 1c00 0000 0048 0c1d 109e 029d  .........H......
+00002920: 0400 0000 0000 0000 1c00 0000 ac00 0000  ................
+00002930: b8f0 ffff d800 0000 0054 0c1d 109e 029d  .........T......
+00002940: 0493 0694 0895 0c00 1c00 0000 cc00 0000  ................
+00002950: 70f1 ffff 6800 0000 0050 0c1d 109e 029d  p...h....P......
+00002960: 0493 0800 0000 0000 1c00 0000 ec00 0000  ................
+00002970: b8f1 ffff 5400 0000 0050 0c1d 109e 029d  ....T....P......
+00002980: 0493 0800 0000 0000 1c00 0000 0c01 0000  ................
+00002990: ecf1 ffff e400 0000 0050 0c1d 109e 029d  .........P......
+000029a0: 0493 0694 0895 0c00 2400 0000 2c01 0000  ........$...,...
+000029b0: b0f2 ffff cc00 0000 0054 0c1d 109e 029d  .........T......
+000029c0: 0493 0694 0895 0a9c 0c00 0000 0000 0000  ................
+000029d0: 2c00 0000 5401 0000 54f3 ffff 1803 0000  ,...T...T.......
+000029e0: 0060 0c1d 109e 029d 0493 0694 0895 0a96  .`..............
+000029f0: 0c97 0e98 1099 129a 149b 1800 0000 0000  ................
+00002a00: 1c00 0000 8401 0000 3cf6 ffff 3001 0000  ........<...0...
+00002a10: 0050 0c1d 109e 029d 0493 0694 0895 0c00  .P..............
+00002a20: 2400 0000 a401 0000 4cf7 ffff d401 0000  $.......L.......
+00002a30: 0054 0c1d 109e 029d 0493 0694 0895 0a96  .T..............
+00002a40: 0c97 0e98 1000 0000 0800 0000 8400 0000  ................
+00002a50: 0100 0000 416e 6472 6f69 6400 1500 0000  ....Android.....
+00002a60: 7231 3662 0000 0000 0000 0000 0000 0000  r16b............
 00002a70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002a80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002a90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002aa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002aa0: 3434 3739 3439 3900 0000 0000 0000 0000  4479499.........
 00002ab0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002ac0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002ad0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002ae0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002af0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002b00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002b10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -704,154 +704,173 @@
 00002bf0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002c00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002c10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002c20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002c30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002c40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002c50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002c60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002c70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002c80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002c90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002ca0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002cb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002cc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002cd0: 0000 0000 0000 0000 0100 0000 0000 0000  ................
-00002ce0: c201 0000 0000 0000 0100 0000 0000 0000  ................
-00002cf0: cc01 0000 0000 0000 0100 0000 0000 0000  ................
-00002d00: d901 0000 0000 0000 0100 0000 0000 0000  ................
-00002d10: e101 0000 0000 0000 0100 0000 0000 0000  ................
-00002d20: e901 0000 0000 0000 0e00 0000 0000 0000  ................
-00002d30: 2c02 0000 0000 0000 1000 0000 0000 0000  ,...............
-00002d40: 0000 0000 0000 0000 1900 0000 0000 0000  ................
-00002d50: c02c 0100 0000 0000 1b00 0000 0000 0000  .,..............
-00002d60: 0800 0000 0000 0000 1a00 0000 0000 0000  ................
-00002d70: c82c 0100 0000 0000 1c00 0000 0000 0000  .,..............
-00002d80: 1000 0000 0000 0000 0400 0000 0000 0000  ................
-00002d90: 9001 0000 0000 0000 0500 0000 0000 0000  ................
-00002da0: f807 0000 0000 0000 0600 0000 0000 0000  ................
-00002db0: 0003 0000 0000 0000 0a00 0000 0000 0000  ................
-00002dc0: 3c02 0000 0000 0000 0b00 0000 0000 0000  <...............
-00002dd0: 1800 0000 0000 0000 0300 0000 0000 0000  ................
-00002de0: c82e 0100 0000 0000 0200 0000 0000 0000  ................
-00002df0: 1803 0000 0000 0000 1400 0000 0000 0000  ................
-00002e00: 0700 0000 0000 0000 1700 0000 0000 0000  ................
-00002e10: 800a 0000 0000 0000 0700 0000 0000 0000  ................
-00002e20: 380a 0000 0000 0000 0800 0000 0000 0000  8...............
-00002e30: 4800 0000 0000 0000 0900 0000 0000 0000  H...............
-00002e40: 1800 0000 0000 0000 1800 0000 0000 0000  ................
-00002e50: 0000 0000 0000 0000 fbff ff6f 0000 0000  ...........o....
-00002e60: 0100 0000 0000 0000 f9ff ff6f 0000 0000  ...........o....
-00002e70: 0200 0000 0000 0000 0000 0000 0000 0000  ................
+00002c60: 0000 0000 0000 0000 2013 0000 0000 0000  ........ .......
+00002c70: 0000 0000 0000 0000 0100 0000 0000 0000  ................
+00002c80: 0002 0000 0000 0000 0100 0000 0000 0000  ................
+00002c90: 0a02 0000 0000 0000 0100 0000 0000 0000  ................
+00002ca0: 1202 0000 0000 0000 0100 0000 0000 0000  ................
+00002cb0: 1a02 0000 0000 0000 0100 0000 0000 0000  ................
+00002cc0: 2702 0000 0000 0000 0e00 0000 0000 0000  '...............
+00002cd0: 6a02 0000 0000 0000 1900 0000 0000 0000  j...............
+00002ce0: 602c 0100 0000 0000 1b00 0000 0000 0000  `,..............
+00002cf0: 0800 0000 0000 0000 1a00 0000 0000 0000  ................
+00002d00: 682c 0100 0000 0000 1c00 0000 0000 0000  h,..............
+00002d10: 1000 0000 0000 0000 0400 0000 0000 0000  ................
+00002d20: 2802 0000 0000 0000 0500 0000 0000 0000  (...............
+00002d30: 0009 0000 0000 0000 0600 0000 0000 0000  ................
+00002d40: a803 0000 0000 0000 0a00 0000 0000 0000  ................
+00002d50: 7f02 0000 0000 0000 0b00 0000 0000 0000  ................
+00002d60: 1800 0000 0000 0000 0300 0000 0000 0000  ................
+00002d70: 882e 0100 0000 0000 0200 0000 0000 0000  ................
+00002d80: f003 0000 0000 0000 1400 0000 0000 0000  ................
+00002d90: 0700 0000 0000 0000 1700 0000 0000 0000  ................
+00002da0: 680c 0000 0000 0000 0700 0000 0000 0000  h...............
+00002db0: 380c 0000 0000 0000 0800 0000 0000 0000  8...............
+00002dc0: 3000 0000 0000 0000 0900 0000 0000 0000  0...............
+00002dd0: 1800 0000 0000 0000 1800 0000 0000 0000  ................
+00002de0: 0000 0000 0000 0000 fbff ff6f 0000 0000  ...........o....
+00002df0: 0100 0000 0000 0000 feff ff6f 0000 0000  ...........o....
+00002e00: f80b 0000 0000 0000 ffff ff6f 0000 0000  ...........o....
+00002e10: 0200 0000 0000 0000 f0ff ff6f 0000 0000  ...........o....
+00002e20: 800b 0000 0000 0000 f9ff ff6f 0000 0000  ...........o....
+00002e30: 0100 0000 0000 0000 0000 0000 0000 0000  ................
+00002e40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002e50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002e60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002e70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002e80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002e90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002ea0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002eb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002ec0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002ed0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002ee0: a00d 0000 0000 0000 a00d 0000 0000 0000  ................
-00002ef0: a00d 0000 0000 0000 a00d 0000 0000 0000  ................
-00002f00: a00d 0000 0000 0000 a00d 0000 0000 0000  ................
-00002f10: a00d 0000 0000 0000 a00d 0000 0000 0000  ................
-00002f20: a00d 0000 0000 0000 a00d 0000 0000 0000  ................
-00002f30: a00d 0000 0000 0000 a00d 0000 0000 0000  ................
-00002f40: a00d 0000 0000 0000 a00d 0000 0000 0000  ................
-00002f50: a00d 0000 0000 0000 a00d 0000 0000 0000  ................
-00002f60: a00d 0000 0000 0000 a00d 0000 0000 0000  ................
-00002f70: a00d 0000 0000 0000 a00d 0000 0000 0000  ................
-00002f80: a00d 0000 0000 0000 a00d 0000 0000 0000  ................
-00002f90: a00d 0000 0000 0000 a00d 0000 0000 0000  ................
-00002fa0: a00d 0000 0000 0000 a00d 0000 0000 0000  ................
-00002fb0: a00d 0000 0000 0000 a00d 0000 0000 0000  ................
-00002fc0: a00d 0000 0000 0000 a00d 0000 0000 0000  ................
-00002fd0: a00d 0000 0000 0000 a00d 0000 0000 0000  ................
-00002fe0: a00d 0000 0000 0000 d82c 0100 0000 0000  .........,......
-00002ff0: 0000 0000 0000 0000 0c10 0000 0000 0000  ................
+00002ea0: 6010 0000 0000 0000 6010 0000 0000 0000  `.......`.......
+00002eb0: 6010 0000 0000 0000 6010 0000 0000 0000  `.......`.......
+00002ec0: 6010 0000 0000 0000 6010 0000 0000 0000  `.......`.......
+00002ed0: 6010 0000 0000 0000 6010 0000 0000 0000  `.......`.......
+00002ee0: 6010 0000 0000 0000 6010 0000 0000 0000  `.......`.......
+00002ef0: 6010 0000 0000 0000 6010 0000 0000 0000  `.......`.......
+00002f00: 6010 0000 0000 0000 6010 0000 0000 0000  `.......`.......
+00002f10: 6010 0000 0000 0000 6010 0000 0000 0000  `.......`.......
+00002f20: 6010 0000 0000 0000 6010 0000 0000 0000  `.......`.......
+00002f30: 6010 0000 0000 0000 6010 0000 0000 0000  `.......`.......
+00002f40: 6010 0000 0000 0000 6010 0000 0000 0000  `.......`.......
+00002f50: 6010 0000 0000 0000 6010 0000 0000 0000  `.......`.......
+00002f60: 6010 0000 0000 0000 6010 0000 0000 0000  `.......`.......
+00002f70: 6010 0000 0000 0000 6010 0000 0000 0000  `.......`.......
+00002f80: 6010 0000 0000 0000 6010 0000 0000 0000  `.......`.......
+00002f90: 6010 0000 0000 0000 6010 0000 0000 0000  `.......`.......
+00002fa0: 6010 0000 0000 0000 6010 0000 0000 0000  `.......`.......
+00002fb0: 6010 0000 0000 0000 6010 0000 0000 0000  `.......`.......
+00002fc0: 6010 0000 0000 0000 6010 0000 0000 0000  `.......`.......
+00002fd0: 6010 0000 0000 0000 6010 0000 0000 0000  `.......`.......
+00002fe0: 6010 0000 0000 0000 6010 0000 0000 0000  `.......`.......
+00002ff0: 782c 0100 0000 0000 0000 0000 0000 0000  x,..............
 00003000: 0000 0000 0000 0000 4743 433a 2028 474e  ........GCC: (GN
-00003010: 5529 2034 2e39 2032 3031 3430 3832 3720  U) 4.9 20140827 
-00003020: 2870 7265 7265 6c65 6173 6529 0000 2e73  (prerelease)...s
-00003030: 6873 7472 7461 6200 2e68 6173 6800 2e64  hstrtab..hash..d
-00003040: 796e 7379 6d00 2e64 796e 7374 7200 2e72  ynsym..dynstr..r
-00003050: 656c 612e 6479 6e00 2e72 656c 612e 706c  ela.dyn..rela.pl
-00003060: 7400 2e74 6578 7400 2e72 6f64 6174 6100  t..text..rodata.
-00003070: 2e65 685f 6672 616d 655f 6864 7200 2e65  .eh_frame_hdr..e
-00003080: 685f 6672 616d 6500 2e69 6e69 745f 6172  h_frame..init_ar
-00003090: 7261 7900 2e66 696e 695f 6172 7261 7900  ray..fini_array.
-000030a0: 2e64 796e 616d 6963 002e 676f 7400 2e64  .dynamic..got..d
-000030b0: 6174 6100 2e62 7373 002e 636f 6d6d 656e  ata..bss..commen
-000030c0: 7400 0000 0000 0000 0000 0000 0000 0000  t...............
-000030d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000030e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000030f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003100: 0000 0000 0000 0000 0b00 0000 0500 0000  ................
-00003110: 0200 0000 0000 0000 9001 0000 0000 0000  ................
-00003120: 9001 0000 0000 0000 7001 0000 0000 0000  ........p.......
-00003130: 0200 0000 0000 0000 0800 0000 0000 0000  ................
-00003140: 0400 0000 0000 0000 1100 0000 0b00 0000  ................
-00003150: 0200 0000 0000 0000 0003 0000 0000 0000  ................
-00003160: 0003 0000 0000 0000 f804 0000 0000 0000  ................
-00003170: 0300 0000 0300 0000 0800 0000 0000 0000  ................
-00003180: 1800 0000 0000 0000 1900 0000 0300 0000  ................
-00003190: 0200 0000 0000 0000 f807 0000 0000 0000  ................
-000031a0: f807 0000 0000 0000 3c02 0000 0000 0000  ........<.......
-000031b0: 0000 0000 0000 0000 0100 0000 0000 0000  ................
-000031c0: 0000 0000 0000 0000 2100 0000 0400 0000  ........!.......
-000031d0: 0200 0000 0000 0000 380a 0000 0000 0000  ........8.......
-000031e0: 380a 0000 0000 0000 4800 0000 0000 0000  8.......H.......
-000031f0: 0200 0000 0000 0000 0800 0000 0000 0000  ................
-00003200: 1800 0000 0000 0000 2b00 0000 0400 0000  ........+.......
-00003210: 4200 0000 0000 0000 800a 0000 0000 0000  B...............
-00003220: 800a 0000 0000 0000 1803 0000 0000 0000  ................
-00003230: 0200 0000 0600 0000 0800 0000 0000 0000  ................
-00003240: 1800 0000 0000 0000 3000 0000 0100 0000  ........0.......
-00003250: 0600 0000 0000 0000 a00d 0000 0000 0000  ................
-00003260: a00d 0000 0000 0000 3002 0000 0000 0000  ........0.......
-00003270: 0000 0000 0000 0000 1000 0000 0000 0000  ................
-00003280: 1000 0000 0000 0000 3500 0000 0100 0000  ........5.......
-00003290: 0600 0000 0000 0000 d00f 0000 0000 0000  ................
-000032a0: d00f 0000 0000 0000 7c0d 0000 0000 0000  ........|.......
-000032b0: 0000 0000 0000 0000 0400 0000 0000 0000  ................
-000032c0: 0000 0000 0000 0000 3b00 0000 0100 0000  ........;.......
-000032d0: 3200 0000 0000 0000 501d 0000 0000 0000  2.......P.......
-000032e0: 501d 0000 0000 0000 0804 0000 0000 0000  P...............
-000032f0: 0000 0000 0000 0000 0800 0000 0000 0000  ................
-00003300: 0100 0000 0000 0000 4300 0000 0100 0000  ........C.......
-00003310: 0200 0000 0000 0000 5821 0000 0000 0000  ........X!......
-00003320: 5821 0000 0000 0000 5400 0000 0000 0000  X!......T.......
-00003330: 0000 0000 0000 0000 0400 0000 0000 0000  ................
-00003340: 0000 0000 0000 0000 5100 0000 0100 0000  ........Q.......
-00003350: 0200 0000 0000 0000 b021 0000 0000 0000  .........!......
-00003360: b021 0000 0000 0000 0002 0000 0000 0000  .!..............
-00003370: 0000 0000 0000 0000 0800 0000 0000 0000  ................
-00003380: 0000 0000 0000 0000 5b00 0000 0e00 0000  ........[.......
-00003390: 0300 0000 0000 0000 c02c 0100 0000 0000  .........,......
-000033a0: c02c 0000 0000 0000 0800 0000 0000 0000  .,..............
-000033b0: 0000 0000 0000 0000 0100 0000 0000 0000  ................
-000033c0: 0000 0000 0000 0000 6700 0000 0f00 0000  ........g.......
-000033d0: 0300 0000 0000 0000 c82c 0100 0000 0000  .........,......
-000033e0: c82c 0000 0000 0000 1000 0000 0000 0000  .,..............
-000033f0: 0000 0000 0000 0000 0800 0000 0000 0000  ................
-00003400: 0000 0000 0000 0000 7300 0000 0600 0000  ........s.......
-00003410: 0300 0000 0000 0000 d82c 0100 0000 0000  .........,......
-00003420: d82c 0000 0000 0000 f001 0000 0000 0000  .,..............
-00003430: 0300 0000 0000 0000 0800 0000 0000 0000  ................
-00003440: 1000 0000 0000 0000 7c00 0000 0100 0000  ........|.......
-00003450: 0300 0000 0000 0000 c82e 0100 0000 0000  ................
-00003460: c82e 0000 0000 0000 3801 0000 0000 0000  ........8.......
-00003470: 0000 0000 0000 0000 0800 0000 0000 0000  ................
-00003480: 0800 0000 0000 0000 8100 0000 0100 0000  ................
-00003490: 0300 0000 0000 0000 0030 0100 0000 0000  .........0......
-000034a0: 0030 0000 0000 0000 0800 0000 0000 0000  .0..............
-000034b0: 0000 0000 0000 0000 0800 0000 0000 0000  ................
-000034c0: 0000 0000 0000 0000 8700 0000 0800 0000  ................
-000034d0: 0300 0000 0000 0000 0830 0100 0000 0000  .........0......
-000034e0: 0830 0000 0000 0000 0000 0000 0000 0000  .0..............
-000034f0: 0000 0000 0000 0000 0100 0000 0000 0000  ................
-00003500: 0000 0000 0000 0000 8c00 0000 0100 0000  ................
-00003510: 3000 0000 0000 0000 0000 0000 0000 0000  0...............
-00003520: 0830 0000 0000 0000 2500 0000 0000 0000  .0......%.......
-00003530: 0000 0000 0000 0000 0100 0000 0000 0000  ................
-00003540: 0100 0000 0000 0000 0100 0000 0300 0000  ................
-00003550: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003560: 2d30 0000 0000 0000 9500 0000 0000 0000  -0..............
-00003570: 0000 0000 0000 0000 0100 0000 0000 0000  ................
-00003580: 0000 0000 0000 0000                      ........
+00003010: 5529 2034 2e39 2e78 2032 3031 3530 3132  U) 4.9.x 2015012
+00003020: 3320 2870 7265 7265 6c65 6173 6529 0041  3 (prerelease).A
+00003030: 6e64 726f 6964 2063 6c61 6e67 2076 6572  ndroid clang ver
+00003040: 7369 6f6e 2035 2e30 2e33 3030 3038 3020  sion 5.0.300080 
+00003050: 2028 6261 7365 6420 6f6e 204c 4c56 4d20   (based on LLVM 
+00003060: 352e 302e 3330 3030 3830 2900 002e 7368  5.0.300080)...sh
+00003070: 7374 7274 6162 002e 6e6f 7465 2e67 6e75  strtab..note.gnu
+00003080: 2e62 7569 6c64 2d69 6400 2e68 6173 6800  .build-id..hash.
+00003090: 2e64 796e 7379 6d00 2e64 796e 7374 7200  .dynsym..dynstr.
+000030a0: 2e67 6e75 2e76 6572 7369 6f6e 002e 676e  .gnu.version..gn
+000030b0: 752e 7665 7273 696f 6e5f 7200 2e72 656c  u.version_r..rel
+000030c0: 612e 6479 6e00 2e72 656c 612e 706c 7400  a.dyn..rela.plt.
+000030d0: 2e74 6578 7400 2e72 6f64 6174 6100 2e65  .text..rodata..e
+000030e0: 685f 6672 616d 655f 6864 7200 2e65 685f  h_frame_hdr..eh_
+000030f0: 6672 616d 6500 2e6e 6f74 652e 616e 6472  frame..note.andr
+00003100: 6f69 642e 6964 656e 7400 2e69 6e69 745f  oid.ident..init_
+00003110: 6172 7261 7900 2e66 696e 695f 6172 7261  array..fini_arra
+00003120: 7900 2e64 796e 616d 6963 002e 676f 7400  y..dynamic..got.
+00003130: 2e64 6174 6100 2e63 6f6d 6d65 6e74 0000  .data..comment..
+00003140: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003150: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003160: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003170: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003180: 0b00 0000 0700 0000 0200 0000 0000 0000  ................
+00003190: 0002 0000 0000 0000 0002 0000 0000 0000  ................
+000031a0: 2400 0000 0000 0000 0000 0000 0000 0000  $...............
+000031b0: 0400 0000 0000 0000 0000 0000 0000 0000  ................
+000031c0: 1e00 0000 0500 0000 0200 0000 0000 0000  ................
+000031d0: 2802 0000 0000 0000 2802 0000 0000 0000  (.......(.......
+000031e0: 8001 0000 0000 0000 0300 0000 0000 0000  ................
+000031f0: 0800 0000 0000 0000 0400 0000 0000 0000  ................
+00003200: 2400 0000 0b00 0000 0200 0000 0000 0000  $...............
+00003210: a803 0000 0000 0000 a803 0000 0000 0000  ................
+00003220: 5805 0000 0000 0000 0400 0000 0300 0000  X...............
+00003230: 0800 0000 0000 0000 1800 0000 0000 0000  ................
+00003240: 2c00 0000 0300 0000 0200 0000 0000 0000  ,...............
+00003250: 0009 0000 0000 0000 0009 0000 0000 0000  ................
+00003260: 7f02 0000 0000 0000 0000 0000 0000 0000  ................
+00003270: 0100 0000 0000 0000 0000 0000 0000 0000  ................
+00003280: 3400 0000 ffff ff6f 0200 0000 0000 0000  4......o........
+00003290: 800b 0000 0000 0000 800b 0000 0000 0000  ................
+000032a0: 7200 0000 0000 0000 0300 0000 0000 0000  r...............
+000032b0: 0200 0000 0000 0000 0200 0000 0000 0000  ................
+000032c0: 4100 0000 feff ff6f 0200 0000 0000 0000  A......o........
+000032d0: f80b 0000 0000 0000 f80b 0000 0000 0000  ................
+000032e0: 4000 0000 0000 0000 0400 0000 0200 0000  @...............
+000032f0: 0800 0000 0000 0000 0000 0000 0000 0000  ................
+00003300: 5000 0000 0400 0000 0200 0000 0000 0000  P...............
+00003310: 380c 0000 0000 0000 380c 0000 0000 0000  8.......8.......
+00003320: 3000 0000 0000 0000 0300 0000 0000 0000  0...............
+00003330: 0800 0000 0000 0000 1800 0000 0000 0000  ................
+00003340: 5a00 0000 0400 0000 4200 0000 0000 0000  Z.......B.......
+00003350: 680c 0000 0000 0000 680c 0000 0000 0000  h.......h.......
+00003360: f003 0000 0000 0000 0300 0000 1200 0000  ................
+00003370: 0800 0000 0000 0000 1800 0000 0000 0000  ................
+00003380: 5f00 0000 0100 0000 0600 0000 0000 0000  _...............
+00003390: 6010 0000 0000 0000 6010 0000 0000 0000  `.......`.......
+000033a0: c002 0000 0000 0000 0000 0000 0000 0000  ................
+000033b0: 1000 0000 0000 0000 1000 0000 0000 0000  ................
+000033c0: 6400 0000 0100 0000 0600 0000 0000 0000  d...............
+000033d0: 2013 0000 0000 0000 2013 0000 0000 0000   ....... .......
+000033e0: 2810 0000 0000 0000 0000 0000 0000 0000  (...............
+000033f0: 0400 0000 0000 0000 0000 0000 0000 0000  ................
+00003400: 6a00 0000 0100 0000 0200 0000 0000 0000  j...............
+00003410: 4823 0000 0000 0000 4823 0000 0000 0000  H#......H#......
+00003420: c504 0000 0000 0000 0000 0000 0000 0000  ................
+00003430: 0100 0000 0000 0000 0000 0000 0000 0000  ................
+00003440: 7200 0000 0100 0000 0200 0000 0000 0000  r...............
+00003450: 1028 0000 0000 0000 1028 0000 0000 0000  .(.......(......
+00003460: 6c00 0000 0000 0000 0000 0000 0000 0000  l...............
+00003470: 0400 0000 0000 0000 0000 0000 0000 0000  ................
+00003480: 8000 0000 0100 0000 0200 0000 0000 0000  ................
+00003490: 8028 0000 0000 0000 8028 0000 0000 0000  .(.......(......
+000034a0: c801 0000 0000 0000 0000 0000 0000 0000  ................
+000034b0: 0800 0000 0000 0000 0000 0000 0000 0000  ................
+000034c0: 8a00 0000 0700 0000 0200 0000 0000 0000  ................
+000034d0: 482a 0000 0000 0000 482a 0000 0000 0000  H*......H*......
+000034e0: 9800 0000 0000 0000 0000 0000 0000 0000  ................
+000034f0: 0400 0000 0000 0000 0000 0000 0000 0000  ................
+00003500: 9e00 0000 0e00 0000 0300 0000 0000 0000  ................
+00003510: 602c 0100 0000 0000 602c 0000 0000 0000  `,......`,......
+00003520: 0800 0000 0000 0000 0000 0000 0000 0000  ................
+00003530: 0100 0000 0000 0000 0800 0000 0000 0000  ................
+00003540: aa00 0000 0f00 0000 0300 0000 0000 0000  ................
+00003550: 682c 0100 0000 0000 682c 0000 0000 0000  h,......h,......
+00003560: 1000 0000 0000 0000 0000 0000 0000 0000  ................
+00003570: 0800 0000 0000 0000 0800 0000 0000 0000  ................
+00003580: b600 0000 0600 0000 0300 0000 0000 0000  ................
+00003590: 782c 0100 0000 0000 782c 0000 0000 0000  x,......x,......
+000035a0: 1002 0000 0000 0000 0400 0000 0000 0000  ................
+000035b0: 0800 0000 0000 0000 1000 0000 0000 0000  ................
+000035c0: bf00 0000 0100 0000 0300 0000 0000 0000  ................
+000035d0: 882e 0100 0000 0000 882e 0000 0000 0000  ................
+000035e0: 7801 0000 0000 0000 0000 0000 0000 0000  x...............
+000035f0: 0800 0000 0000 0000 0800 0000 0000 0000  ................
+00003600: c400 0000 0100 0000 0300 0000 0000 0000  ................
+00003610: 0030 0100 0000 0000 0030 0000 0000 0000  .0.......0......
+00003620: 0800 0000 0000 0000 0000 0000 0000 0000  ................
+00003630: 0800 0000 0000 0000 0000 0000 0000 0000  ................
+00003640: ca00 0000 0100 0000 3000 0000 0000 0000  ........0.......
+00003650: 0000 0000 0000 0000 0830 0000 0000 0000  .........0......
+00003660: 6400 0000 0000 0000 0000 0000 0000 0000  d...............
+00003670: 0100 0000 0000 0000 0100 0000 0000 0000  ................
+00003680: 0100 0000 0300 0000 0000 0000 0000 0000  ................
+00003690: 0000 0000 0000 0000 6c30 0000 0000 0000  ........l0......
+000036a0: d300 0000 0000 0000 0000 0000 0000 0000  ................
+000036b0: 0100 0000 0000 0000 0000 0000 0000 0000  ................
```

#### readelf --wide --decompress --hex-dump=.eh_frame_hdr {}

```diff
@@ -1,9 +1,10 @@
 
 Hex dump of section '.eh_frame_hdr':
-  0x00002158 011b033b 54000000 09000000 b4eeffff ...;T...........
-  0x00002168 70000000 0cf2ffff b0000000 48f5ffff p...........H...
-  0x00002178 00010000 4cf5ffff 18010000 6cf5ffff ....L.......l...
-  0x00002188 38010000 b8f5ffff 60010000 a8f6ffff 8.......`.......
-  0x00002198 90010000 8cf7ffff d0010000 c0faffff ................
-  0x000021a8 10020000                            ....
+  0x00002810 011b033b 6c000000 0c000000 4cebffff ...;l.......L...
+  0x00002820 88000000 cceeffff b0000000 b8f1ffff ................
+  0x00002830 e0000000 bcf1ffff f8000000 d8f1ffff ................
+  0x00002840 18010000 b0f2ffff 38010000 18f3ffff ........8.......
+  0x00002850 58010000 6cf3ffff 78010000 50f4ffff X...l...x...P...
+  0x00002860 98010000 1cf5ffff c0010000 34f8ffff ............4...
+  0x00002870 f0010000 64f9ffff 10020000          ....d.......
```

#### readelf --wide --decompress --hex-dump=.eh_frame {}

```diff
@@ -1,35 +1,32 @@
 
 Hex dump of section '.eh_frame':
-  0x000021b0 14000000 00000000 017a5200 04781e01 .........zR..x..
-  0x000021c0 1b0c1f00 00000000 3c000000 1c000000 ........<.......
-  0x000021d0 3ceeffff 58030000 00410e60 43950a96 <...X....A.`C...
-  0x000021e0 0944930c 940b9708 98074299 069e0502 .D........B.....
-  0x000021f0 9d0ad4d3 41d6d541 d8d741de d9410e00 ....A..A..A..A..
-  0x00002200 410b0000 00000000 4c000000 5c000000 A.......L...\...
-  0x00002210 54f1ffff 3c030000 00410ec0 06410ea0 T...<....A...A..
-  0x00002220 07419572 9671459e 6a977098 6f996e9a .A.r.qE.j.p.o.n.
-  0x00002230 6d439374 94739b6c 9c6b029e 0ad4d341 mC.t.s.l.k.....A
-  0x00002240 d6d541d8 d741dad9 41dcdb41 de410ec0 ..A..A..A..A.A..
-  0x00002250 06410ee0 05410b00 14000000 ac000000 .A...A..........
-  0x00002260 40f4ffff 04000000 00000000 00000000 @...............
-  0x00002270 1c000000 c4000000 2cf4ffff 20000000 ........,... ...
-  0x00002280 00410e10 429e0243 de410e00 00000000 .A..B..C.A......
-  0x00002290 24000000 e4000000 2cf4ffff 4c000000 $.......,...L...
-  0x000022a0 00410ea0 01429314 9e134d0a ded3410e .A...B....M...A.
-  0x000022b0 00410b00 00000000 2c000000 0c010000 .A......,.......
-  0x000022c0 50f4ffff f0000000 00410e30 44950496 P........A.0D...
-  0x000022d0 03469306 9405439e 025a0ad4 d341d6d5 .F....C..Z...A..
-  0x000022e0 41de410e 00410b00 3c000000 3c010000 A.A..A..<...<...
-  0x000022f0 10f5ffff e4000000 00410e90 08420ec0 .........A...B..
-  0x00002300 08429586 01968501 439e8401 93880194 .B......C.......
-  0x00002310 87015e0a d4d341d6 d541de41 0e900841 ..^...A..A.A...A
-  0x00002320 0ee00741 0b000000 3c000000 7c010000 ...A....<...|...
-  0x00002330 b4f5ffff 34030000 00410ee0 0141931c ....4....A...A..
-  0x00002340 941b459e 14951a96 19971898 17429916 ..E..........B..
-  0x00002350 9a150296 0ad4d341 d6d541d8 d741dad9 .......A..A..A..
-  0x00002360 41de410e 00410b00 44000000 bc010000 A.A..A..D.......
-  0x00002370 a8f8ffff 34010000 00410e40 42930894 ....4....A.@B...
-  0x00002380 07469e02 95069605 97049803 4c0ad4d3 .F..........L...
-  0x00002390 41d6d541 d8d741de 410e0041 0b5e0ade A..A..A.A..A.^..
-  0x000023a0 41d3d441 d5d641d7 d8410e00 410b0000 A..A..A..A..A...
+  0x00002880 14000000 00000000 017a5200 017c1e01 .........zR..|..
+  0x00002890 1b0c1f00 00000000 24000000 1c000000 ........$.......
+  0x000028a0 bceaffff 80030000 005c0c1d 109e029d .........\......
+  0x000028b0 04930694 08950a96 0c970e98 10991400 ................
+  0x000028c0 2c000000 44000000 14eeffff ec020000 ,...D...........
+  0x000028d0 00600c1d 109e029d 04930694 08950a96 .`..............
+  0x000028e0 0c970e98 1099129a 149c1800 00000000 ................
+  0x000028f0 14000000 74000000 d0f0ffff 04000000 ....t...........
+  0x00002900 00000000 00000000 1c000000 8c000000 ................
+  0x00002910 bcf0ffff 1c000000 00480c1d 109e029d .........H......
+  0x00002920 04000000 00000000 1c000000 ac000000 ................
+  0x00002930 b8f0ffff d8000000 00540c1d 109e029d .........T......
+  0x00002940 04930694 08950c00 1c000000 cc000000 ................
+  0x00002950 70f1ffff 68000000 00500c1d 109e029d p...h....P......
+  0x00002960 04930800 00000000 1c000000 ec000000 ................
+  0x00002970 b8f1ffff 54000000 00500c1d 109e029d ....T....P......
+  0x00002980 04930800 00000000 1c000000 0c010000 ................
+  0x00002990 ecf1ffff e4000000 00500c1d 109e029d .........P......
+  0x000029a0 04930694 08950c00 24000000 2c010000 ........$...,...
+  0x000029b0 b0f2ffff cc000000 00540c1d 109e029d .........T......
+  0x000029c0 04930694 08950a9c 0c000000 00000000 ................
+  0x000029d0 2c000000 54010000 54f3ffff 18030000 ,...T...T.......
+  0x000029e0 00600c1d 109e029d 04930694 08950a96 .`..............
+  0x000029f0 0c970e98 1099129a 149b1800 00000000 ................
+  0x00002a00 1c000000 84010000 3cf6ffff 30010000 ........<...0...
+  0x00002a10 00500c1d 109e029d 04930694 08950c00 .P..............
+  0x00002a20 24000000 a4010000 4cf7ffff d4010000 $.......L.......
+  0x00002a30 00540c1d 109e029d 04930694 08950a96 .T..............
+  0x00002a40 0c970e98 10000000                   ........
```

#### readelf --wide --decompress --hex-dump=.init_array {}

```diff
@@ -1,4 +1,4 @@
 
 Hex dump of section '.init_array':
-  0x00012cc0 00000000 00000000                   ........
+  0x00012c60 00000000 00000000                   ........
```

#### readelf --wide --decompress --hex-dump=.fini_array {}

```diff
@@ -1,4 +1,4 @@
 
 Hex dump of section '.fini_array':
-  0x00012cc8 00000000 00000000 00000000 00000000 ................
+  0x00012c68 20130000 00000000 00000000 00000000  ...............
```

#### readelf --wide --decompress --hex-dump=.got {}

```diff
@@ -1,23 +1,28 @@
 
 Hex dump of section '.got':
-  0x00012ec8 00000000 00000000 00000000 00000000 ................
-  0x00012ed8 00000000 00000000 a00d0000 00000000 ................
-  0x00012ee8 a00d0000 00000000 a00d0000 00000000 ................
-  0x00012ef8 a00d0000 00000000 a00d0000 00000000 ................
-  0x00012f08 a00d0000 00000000 a00d0000 00000000 ................
-  0x00012f18 a00d0000 00000000 a00d0000 00000000 ................
-  0x00012f28 a00d0000 00000000 a00d0000 00000000 ................
-  0x00012f38 a00d0000 00000000 a00d0000 00000000 ................
-  0x00012f48 a00d0000 00000000 a00d0000 00000000 ................
-  0x00012f58 a00d0000 00000000 a00d0000 00000000 ................
-  0x00012f68 a00d0000 00000000 a00d0000 00000000 ................
-  0x00012f78 a00d0000 00000000 a00d0000 00000000 ................
-  0x00012f88 a00d0000 00000000 a00d0000 00000000 ................
-  0x00012f98 a00d0000 00000000 a00d0000 00000000 ................
-  0x00012fa8 a00d0000 00000000 a00d0000 00000000 ................
-  0x00012fb8 a00d0000 00000000 a00d0000 00000000 ................
-  0x00012fc8 a00d0000 00000000 a00d0000 00000000 ................
-  0x00012fd8 a00d0000 00000000 a00d0000 00000000 ................
-  0x00012fe8 d82c0100 00000000 00000000 00000000 .,..............
-  0x00012ff8 0c100000 00000000                   ........
+ NOTE: This section has relocations against it, but these have NOT been applied to this dump.
+  0x00012e88 00000000 00000000 00000000 00000000 ................
+  0x00012e98 00000000 00000000 60100000 00000000 ........`.......
+  0x00012ea8 60100000 00000000 60100000 00000000 `.......`.......
+  0x00012eb8 60100000 00000000 60100000 00000000 `.......`.......
+  0x00012ec8 60100000 00000000 60100000 00000000 `.......`.......
+  0x00012ed8 60100000 00000000 60100000 00000000 `.......`.......
+  0x00012ee8 60100000 00000000 60100000 00000000 `.......`.......
+  0x00012ef8 60100000 00000000 60100000 00000000 `.......`.......
+  0x00012f08 60100000 00000000 60100000 00000000 `.......`.......
+  0x00012f18 60100000 00000000 60100000 00000000 `.......`.......
+  0x00012f28 60100000 00000000 60100000 00000000 `.......`.......
+  0x00012f38 60100000 00000000 60100000 00000000 `.......`.......
+  0x00012f48 60100000 00000000 60100000 00000000 `.......`.......
+  0x00012f58 60100000 00000000 60100000 00000000 `.......`.......
+  0x00012f68 60100000 00000000 60100000 00000000 `.......`.......
+  0x00012f78 60100000 00000000 60100000 00000000 `.......`.......
+  0x00012f88 60100000 00000000 60100000 00000000 `.......`.......
+  0x00012f98 60100000 00000000 60100000 00000000 `.......`.......
+  0x00012fa8 60100000 00000000 60100000 00000000 `.......`.......
+  0x00012fb8 60100000 00000000 60100000 00000000 `.......`.......
+  0x00012fc8 60100000 00000000 60100000 00000000 `.......`.......
+  0x00012fd8 60100000 00000000 60100000 00000000 `.......`.......
+  0x00012fe8 60100000 00000000 782c0100 00000000 `.......x,......
+  0x00012ff8 00000000 00000000                   ........
```

#### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,5 @@
 
 String dump of section '.comment':
-  [     0]  GCC: (GNU) 4.9 20140827 (prerelease)
+  [     0]  GCC: (GNU) 4.9.x 20150123 (prerelease)
+  [    27]  Android clang version 5.0.300080  (based on LLVM 5.0.300080)
```

#### readelf --wide --decompress --hex-dump=.shstrtab {}

```diff
@@ -1,13 +1,17 @@
 
 Hex dump of section '.shstrtab':
-  0x00000000 002e7368 73747274 6162002e 68617368 ..shstrtab..hash
-  0x00000010 002e6479 6e73796d 002e6479 6e737472 ..dynsym..dynstr
-  0x00000020 002e7265 6c612e64 796e002e 72656c61 ..rela.dyn..rela
-  0x00000030 2e706c74 002e7465 7874002e 726f6461 .plt..text..roda
-  0x00000040 7461002e 65685f66 72616d65 5f686472 ta..eh_frame_hdr
-  0x00000050 002e6568 5f667261 6d65002e 696e6974 ..eh_frame..init
-  0x00000060 5f617272 6179002e 66696e69 5f617272 _array..fini_arr
-  0x00000070 6179002e 64796e61 6d696300 2e676f74 ay..dynamic..got
-  0x00000080 002e6461 7461002e 62737300 2e636f6d ..data..bss..com
-  0x00000090 6d656e74 00                         ment.
+  0x00000000 002e7368 73747274 6162002e 6e6f7465 ..shstrtab..note
+  0x00000010 2e676e75 2e627569 6c642d69 64002e68 .gnu.build-id..h
+  0x00000020 61736800 2e64796e 73796d00 2e64796e ash..dynsym..dyn
+  0x00000030 73747200 2e676e75 2e766572 73696f6e str..gnu.version
+  0x00000040 002e676e 752e7665 7273696f 6e5f7200 ..gnu.version_r.
+  0x00000050 2e72656c 612e6479 6e002e72 656c612e .rela.dyn..rela.
+  0x00000060 706c7400 2e746578 74002e72 6f646174 plt..text..rodat
+  0x00000070 61002e65 685f6672 616d655f 68647200 a..eh_frame_hdr.
+  0x00000080 2e65685f 6672616d 65002e6e 6f74652e .eh_frame..note.
+  0x00000090 616e6472 6f69642e 6964656e 74002e69 android.ident..i
+  0x000000a0 6e69745f 61727261 79002e66 696e695f nit_array..fini_
+  0x000000b0 61727261 79002e64 796e616d 6963002e array..dynamic..
+  0x000000c0 676f7400 2e646174 61002e63 6f6d6d65 got..data..comme
+  0x000000d0 6e7400                              nt.
```

### Comparing `qt4a-2.3.1/qt4a/androiddriver/tools/arm64-v8a/screenkit` & `qt4a-3.0.0/qt4a/androiddriver/tools/arm64-v8a/screenkit`

 * *Files identical despite different names*

### Comparing `qt4a-2.3.1/qt4a/androiddriver/tools/armeabi/droid_inject` & `qt4a-3.0.0/qt4a/androiddriver/tools/armeabi/droid_inject`

 * *Files identical despite different names*

### Comparing `qt4a-2.3.1/qt4a/androiddriver/tools/armeabi/screenkit` & `qt4a-3.0.0/qt4a/androiddriver/tools/armeabi/screenkit`

 * *Files identical despite different names*

### Comparing `qt4a-2.3.1/qt4a/androiddriver/tools/armeabi-v7a/droid_inject` & `qt4a-3.0.0/qt4a/androiddriver/tools/armeabi-v7a/droid_inject`

 * *Files identical despite different names*

### Comparing `qt4a-2.3.1/qt4a/androiddriver/tools/armeabi-v7a/screenkit` & `qt4a-3.0.0/qt4a/androiddriver/tools/armeabi-v7a/screenkit`

 * *Files identical despite different names*

### Comparing `qt4a-2.3.1/qt4a/androiddriver/tools/x86/droid_inject` & `qt4a-3.0.0/qt4a/androiddriver/tools/x86/droid_inject`

 * *Files identical despite different names*

### Comparing `qt4a-2.3.1/qt4a/androiddriver/tools/x86/libdexloader.so` & `qt4a-3.0.0/qt4a/androiddriver/tools/x86_64/droid_inject`

 * *Files 26% similar despite different names*

#### readelf --wide --file-header {}

```diff
@@ -4,17 +4,17 @@
   Data:                              2's complement, little endian
   Version:                           1 (current)
   OS/ABI:                            UNIX - System V
   ABI Version:                       0
   Type:                              DYN (Shared object file)
   Machine:                           Intel 80386
   Version:                           0x1
-  Entry point address:               0x0
+  Entry point address:               0x1090
   Start of program headers:          52 (bytes into file)
-  Start of section headers:          12516 (bytes into file)
+  Start of section headers:          17548 (bytes into file)
   Flags:                             0x0
   Size of this header:               52 (bytes)
   Size of program headers:           32 (bytes)
-  Number of program headers:         7
+  Number of program headers:         8
   Size of section headers:           40 (bytes)
-  Number of section headers:         21
-  Section header string table index: 20
+  Number of section headers:         24
+  Section header string table index: 23
```

#### readelf --wide --program-header {}

```diff
@@ -1,24 +1,27 @@
 
 Elf file type is DYN (Shared object file)
-Entry point 0x0
-There are 7 program headers, starting at offset 52
+Entry point 0x1090
+There are 8 program headers, starting at offset 52
 
 Program Headers:
   Type           Offset   VirtAddr   PhysAddr   FileSiz MemSiz  Flg Align
-  PHDR           0x000034 0x00000034 0x00000034 0x000e0 0x000e0 R   0x4
-  LOAD           0x000000 0x00000000 0x00000000 0x02190 0x02190 R E 0x1000
-  LOAD           0x002e5c 0x00003e5c 0x00003e5c 0x001a8 0x001a8 RW  0x1000
-  DYNAMIC        0x002e68 0x00003e68 0x00003e68 0x00100 0x00100 RW  0x4
-  GNU_EH_FRAME   0x00210c 0x0000210c 0x0000210c 0x00084 0x00084 R   0x4
+  PHDR           0x000034 0x00000034 0x00000034 0x00100 0x00100 R   0x4
+  INTERP         0x000134 0x00000134 0x00000134 0x00013 0x00013 R   0x1
+      [Requesting program interpreter: /system/bin/linker]
+  LOAD           0x000000 0x00000000 0x00000000 0x03c58 0x03c58 R E 0x1000
+  LOAD           0x003e14 0x00004e14 0x00004e14 0x0056c 0x00574 RW  0x1000
+  DYNAMIC        0x003e2c 0x00004e2c 0x00004e2c 0x00108 0x00108 RW  0x4
+  GNU_EH_FRAME   0x003b5c 0x00003b5c 0x00003b5c 0x000fc 0x000fc R   0x4
   GNU_STACK      0x000000 0x00000000 0x00000000 0x00000 0x00000 RW  0
-  GNU_RELRO      0x002e5c 0x00003e5c 0x00003e5c 0x001a4 0x001a4 RW  0x4
+  GNU_RELRO      0x003e14 0x00004e14 0x00004e14 0x001ec 0x001ec RW  0x4
 
  Section to Segment mapping:
   Segment Sections...
    00     
-   01     .dynsym .dynstr .hash .rel.dyn .rel.plt .plt .text .rodata .eh_frame .eh_frame_hdr 
-   02     .fini_array .init_array .dynamic .got .got.plt .data 
-   03     .dynamic 
-   04     .eh_frame_hdr 
-   05     
-   06     .fini_array .init_array .dynamic .got .got.plt 
+   01     .interp 
+   02     .interp .dynsym .dynstr .hash .rel.dyn .rel.plt .plt .text .note.android.ident .rodata .eh_frame .eh_frame_hdr 
+   03     .fini_array .init_array .preinit_array .dynamic .got .got.plt .data .bss 
+   04     .dynamic 
+   05     .eh_frame_hdr 
+   06     
+   07     .fini_array .init_array .preinit_array .dynamic .got .got.plt
```

#### readelf --wide --sections {}

```diff
@@ -1,30 +1,33 @@
-There are 21 section headers, starting at offset 0x30e4:
+There are 24 section headers, starting at offset 0x448c:
 
 Section Headers:
   [Nr] Name              Type            Addr     Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            00000000 000000 000000 00      0   0  0
-  [ 1] .dynsym           DYNSYM          00000114 000114 0002f0 10   A  2   1  4
-  [ 2] .dynstr           STRTAB          00000404 000404 00022f 00   A  0   0  1
-  [ 3] .hash             HASH            00000634 000634 000158 04   A  1   0  4
-  [ 4] .rel.dyn          REL             0000078c 00078c 000020 08   A  1   0  4
-  [ 5] .rel.plt          REL             000007ac 0007ac 000108 08  AI  1   6  4
-  [ 6] .plt              PROGBITS        000008c0 0008c0 000220 04  AX  0   0 16
-  [ 7] .text             PROGBITS        00000ae0 000ae0 000f72 00  AX  0   0 16
-  [ 8] .rodata           PROGBITS        00001a54 001a54 000378 01 AMS  0   0  4
-  [ 9] .eh_frame         PROGBITS        00001dcc 001dcc 000340 00   A  0   0  4
-  [10] .eh_frame_hdr     PROGBITS        0000210c 00210c 000084 00   A  0   0  4
-  [11] .fini_array       FINI_ARRAY      00003e5c 002e5c 000008 00  WA  0   0  4
-  [12] .init_array       INIT_ARRAY      00003e64 002e64 000004 00  WA  0   0  1
-  [13] .dynamic          DYNAMIC         00003e68 002e68 000100 08  WA  2   0  4
-  [14] .got              PROGBITS        00003f68 002f68 000008 00  WA  0   0  4
-  [15] .got.plt          PROGBITS        00003f70 002f70 000090 00  WA  0   0  4
-  [16] .data             PROGBITS        00004000 003000 000004 00  WA  0   0  4
-  [17] .bss              NOBITS          00004004 003004 000000 00  WA  0   0  1
-  [18] .comment          PROGBITS        00000000 003004 000010 01  MS  0   0  1
-  [19] .note.gnu.gold-version NOTE            00000000 003014 00001c 00      0   0  4
-  [20] .shstrtab         STRTAB          00000000 003030 0000b3 00      0   0  1
+  [ 1] .interp           PROGBITS        00000134 000134 000013 00   A  0   0  1
+  [ 2] .dynsym           DYNSYM          00000148 000148 0002f0 10   A  3   1  4
+  [ 3] .dynstr           STRTAB          00000438 000438 0001b0 00   A  0   0  1
+  [ 4] .hash             HASH            000005e8 0005e8 000158 04   A  2   0  4
+  [ 5] .rel.dyn          REL             00000740 000740 000068 08   A  2   0  4
+  [ 6] .rel.plt          REL             000007a8 0007a8 000140 08  AI  2   7  4
+  [ 7] .plt              PROGBITS        000008f0 0008f0 000290 04  AX  0   0 16
+  [ 8] .text             PROGBITS        00000b80 000b80 0021b0 00  AX  0   0 16
+  [ 9] .note.android.ident PROGBITS        00002d30 002d30 000018 00   A  0   0  4
+  [10] .rodata           PROGBITS        00002d48 002d48 000778 00   A  0   0  4
+  [11] .eh_frame         PROGBITS        000034c0 0034c0 00069c 00   A  0   0  4
+  [12] .eh_frame_hdr     PROGBITS        00003b5c 003b5c 0000fc 00   A  0   0  4
+  [13] .fini_array       FINI_ARRAY      00004e14 003e14 000008 00  WA  0   0  4
+  [14] .init_array       INIT_ARRAY      00004e1c 003e1c 000008 00  WA  0   0  4
+  [15] .preinit_array    PREINIT_ARRAY   00004e24 003e24 000008 00  WA  0   0  4
+  [16] .dynamic          DYNAMIC         00004e2c 003e2c 000108 08  WA  3   0  4
+  [17] .got              PROGBITS        00004f34 003f34 000020 00  WA  0   0  4
+  [18] .got.plt          PROGBITS        00004f54 003f54 0000ac 00  WA  0   0  4
+  [19] .data             PROGBITS        00005000 004000 000380 00  WA  0   0 32
+  [20] .bss              NOBITS          00005380 004380 000008 00  WA  0   0  4
+  [21] .comment          PROGBITS        00000000 004380 000010 01  MS  0   0  1
+  [22] .note.gnu.gold-version NOTE            00000000 004390 00001c 00      0   0  4
+  [23] .shstrtab         STRTAB          00000000 0043ac 0000de 00      0   0  1
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
   D (mbind), p (processor specific)
```

#### readelf --wide --symbols {}

```diff
@@ -1,50 +1,50 @@
 
 Symbol table '.dynsym' contains 47 entries:
    Num:    Value  Size Type    Bind   Vis      Ndx Name
      0: 00000000     0 NOTYPE  LOCAL  DEFAULT  UND 
-     1: 00000000     0 FUNC    GLOBAL DEFAULT  UND __cxa_finalize
+     1: 00000000     0 FUNC    GLOBAL DEFAULT  UND __libc_init
      2: 00000000     0 FUNC    GLOBAL DEFAULT  UND __cxa_atexit
      3: 00000000     0 FUNC    GLOBAL DEFAULT  UND __stack_chk_fail
-     4: 00000ba0   853 FUNC    GLOBAL DEFAULT    7 load_dex_in_thread
-     5: 00000000     0 FUNC    GLOBAL DEFAULT  UND __android_log_print
-     6: 00000000     0 FUNC    GLOBAL DEFAULT  UND free
-     7: 00000f00   990 FUNC    GLOBAL DEFAULT    7 load_dex
-     8: 00000000     0 OBJECT  GLOBAL DEFAULT  UND __stack_chk_guard
-     9: 00000000     0 FUNC    GLOBAL DEFAULT  UND strncpy
-    10: 00000000     0 FUNC    GLOBAL DEFAULT  UND getuid
-    11: 00000000     0 FUNC    GLOBAL DEFAULT  UND sprintf
-    12: 00000000     0 FUNC    GLOBAL DEFAULT  UND access
-    13: 00001330    61 FUNC    GLOBAL DEFAULT    7 get_file_size
-    14: 00001910   322 FUNC    GLOBAL DEFAULT    7 get_jni_env
-    15: 00000000     0 FUNC    GLOBAL DEFAULT  UND malloc
-    16: 00000000     0 FUNC    GLOBAL DEFAULT  UND pthread_create
-    17: 00000000     0 FUNC    GLOBAL DEFAULT  UND chmod
-    18: 00001370   227 FUNC    GLOBAL DEFAULT    7 copyfile
-    19: 00000000     0 FUNC    GLOBAL DEFAULT  UND mkdir
-    20: 000012e0    27 FUNC    GLOBAL DEFAULT    7 Java_com_test_androidspy_HelperUtil_nativeSetsid
-    21: 00000000     0 FUNC    GLOBAL DEFAULT  UND setsid
-    22: 00001300    37 FUNC    GLOBAL DEFAULT    7 Java_com_test_androidspy_HelperUtil_nativeUmask
-    23: 00000000     0 FUNC    GLOBAL DEFAULT  UND umask
-    24: 00000000     0 FUNC    GLOBAL DEFAULT  UND stat
-    25: 00000000     0 FUNC    GLOBAL DEFAULT  UND fopen
-    26: 00000000     0 FUNC    GLOBAL DEFAULT  UND fputc
-    27: 00000000     0 FUNC    GLOBAL DEFAULT  UND getc
-    28: 00000000     0 FUNC    GLOBAL DEFAULT  UND fclose
-    29: 00001460   245 FUNC    GLOBAL DEFAULT    7 get_module_base
-    30: 00000000     0 FUNC    GLOBAL DEFAULT  UND strstr
-    31: 00000000     0 FUNC    GLOBAL DEFAULT  UND fgets
-    32: 00000000     0 FUNC    GLOBAL DEFAULT  UND strtok
-    33: 00000000     0 FUNC    GLOBAL DEFAULT  UND strtoul
-    34: 00001560   934 FUNC    GLOBAL DEFAULT    7 get_symbol_offset
-    35: 00000000     0 FUNC    GLOBAL DEFAULT  UND open
-    36: 00000000     0 FUNC    GLOBAL DEFAULT  UND fstat
-    37: 00000000     0 FUNC    GLOBAL DEFAULT  UND mmap
-    38: 00000000     0 FUNC    GLOBAL DEFAULT  UND memset
-    39: 00000000     0 FUNC    GLOBAL DEFAULT  UND read
-    40: 00000000     0 FUNC    GLOBAL DEFAULT  UND close
-    41: 00000000     0 FUNC    GLOBAL DEFAULT  UND strcmp
-    42: 00000000     0 FUNC    GLOBAL DEFAULT  UND munmap
-    43: 00000000     0 FUNC    GLOBAL DEFAULT  UND dlsym
-    44: 00004004     0 NOTYPE  GLOBAL DEFAULT  ABS _edata
-    45: 00004004     0 NOTYPE  GLOBAL DEFAULT  ABS __bss_start
-    46: 00004004     0 NOTYPE  GLOBAL DEFAULT  ABS _end
+     4: 00000000     0 OBJECT  GLOBAL DEFAULT  UND __stack_chk_guard
+     5: 00000000     0 FUNC    GLOBAL DEFAULT  UND __system_property_get
+     6: 00000000     0 FUNC    GLOBAL DEFAULT  UND atoi
+     7: 00000000     0 FUNC    GLOBAL DEFAULT  UND printf
+     8: 00000000     0 FUNC    GLOBAL DEFAULT  UND __android_log_print
+     9: 00000000     0 FUNC    GLOBAL DEFAULT  UND ptrace
+    10: 00000000     0 FUNC    GLOBAL DEFAULT  UND memcpy
+    11: 00000000     0 FUNC    GLOBAL DEFAULT  UND strlen
+    12: 00000000     0 FUNC    GLOBAL DEFAULT  UND perror
+    13: 00000000     0 FUNC    GLOBAL DEFAULT  UND waitpid
+    14: 00000000     0 FUNC    GLOBAL DEFAULT  UND snprintf
+    15: 00000000     0 FUNC    GLOBAL DEFAULT  UND fopen
+    16: 00000000     0 FUNC    GLOBAL DEFAULT  UND strstr
+    17: 00000000     0 FUNC    GLOBAL DEFAULT  UND fgets
+    18: 00000000     0 FUNC    GLOBAL DEFAULT  UND fclose
+    19: 00000000     0 FUNC    GLOBAL DEFAULT  UND strtok
+    20: 00000000     0 FUNC    GLOBAL DEFAULT  UND strtoul
+    21: 00000000     0 FUNC    GLOBAL DEFAULT  UND open
+    22: 00000000     0 FUNC    GLOBAL DEFAULT  UND fstat
+    23: 00000000     0 FUNC    GLOBAL DEFAULT  UND malloc
+    24: 00000000     0 FUNC    GLOBAL DEFAULT  UND memset
+    25: 00000000     0 FUNC    GLOBAL DEFAULT  UND read
+    26: 00000000     0 FUNC    GLOBAL DEFAULT  UND close
+    27: 00000000     0 FUNC    GLOBAL DEFAULT  UND strcmp
+    28: 00000000     0 FUNC    GLOBAL DEFAULT  UND free
+    29: 00000000     0 OBJECT  GLOBAL DEFAULT  UND __sF
+    30: 00000000     0 FUNC    GLOBAL DEFAULT  UND fprintf
+    31: 00000000     0 FUNC    GLOBAL DEFAULT  UND dlopen
+    32: 00000000     0 FUNC    GLOBAL DEFAULT  UND dlsym
+    33: 00000000     0 FUNC    GLOBAL DEFAULT  UND opendir
+    34: 00000000     0 FUNC    GLOBAL DEFAULT  UND readdir
+    35: 00000000     0 FUNC    GLOBAL DEFAULT  UND closedir
+    36: 00000000     0 FUNC    GLOBAL DEFAULT  UND sprintf
+    37: 00000000     0 FUNC    GLOBAL DEFAULT  UND fwrite
+    38: 00000000     0 FUNC    GLOBAL DEFAULT  UND readlink
+    39: 00000000     0 FUNC    GLOBAL DEFAULT  UND lstat
+    40: 00000000     0 FUNC    GLOBAL DEFAULT  UND getopt_long
+    41: 00000000     0 OBJECT  GLOBAL DEFAULT  UND optarg
+    42: 00000000     0 FUNC    GLOBAL DEFAULT  UND fputc
+    43: 00000000     0 FUNC    GLOBAL DEFAULT  UND puts
+    44: 00005380     0 NOTYPE  GLOBAL DEFAULT  ABS _edata
+    45: 00005380     0 NOTYPE  GLOBAL DEFAULT  ABS __bss_start
+    46: 00005388     0 NOTYPE  GLOBAL DEFAULT  ABS _end
```

#### readelf --wide --relocs {}

```diff
@@ -1,43 +1,59 @@
 
-Relocation section '.rel.dyn' at offset 0x78c contains 4 entries:
+Relocation section '.rel.dyn' at offset 0x740 contains 13 entries:
  Offset     Info    Type                Sym. Value  Symbol's Name
-00003e5c  00000008 R_386_RELATIVE        
-00003f6c  00000008 R_386_RELATIVE        
-00004000  00000008 R_386_RELATIVE        
-00003f68  00000806 R_386_GLOB_DAT         00000000   __stack_chk_guard
+00004f34  00000008 R_386_RELATIVE        
+00004f38  00000008 R_386_RELATIVE        
+00004f3c  00000008 R_386_RELATIVE        
+00004f40  00000008 R_386_RELATIVE        
+00005000  00000008 R_386_RELATIVE        
+00005010  00000008 R_386_RELATIVE        
+00005020  00000008 R_386_RELATIVE        
+00005030  00000008 R_386_RELATIVE        
+00005040  00000008 R_386_RELATIVE        
+00004f44  00000406 R_386_GLOB_DAT         00000000   __stack_chk_guard
+00004f48  00001d06 R_386_GLOB_DAT         00000000   __sF
+00004f4c  00001f06 R_386_GLOB_DAT         00000000   dlopen
+00004f50  00002906 R_386_GLOB_DAT         00000000   optarg
 
-Relocation section '.rel.plt' at offset 0x7ac contains 33 entries:
+Relocation section '.rel.plt' at offset 0x7a8 contains 40 entries:
  Offset     Info    Type                Sym. Value  Symbol's Name
-00003f7c  00000207 R_386_JUMP_SLOT        00000000   __cxa_atexit
-00003f80  00000307 R_386_JUMP_SLOT        00000000   __stack_chk_fail
-00003f84  00000107 R_386_JUMP_SLOT        00000000   __cxa_finalize
-00003f88  00000507 R_386_JUMP_SLOT        00000000   __android_log_print
-00003f8c  00000607 R_386_JUMP_SLOT        00000000   free
-00003f90  00000907 R_386_JUMP_SLOT        00000000   strncpy
-00003f94  00000a07 R_386_JUMP_SLOT        00000000   getuid
-00003f98  00000b07 R_386_JUMP_SLOT        00000000   sprintf
-00003f9c  00000c07 R_386_JUMP_SLOT        00000000   access
-00003fa0  00000f07 R_386_JUMP_SLOT        00000000   malloc
-00003fa4  00001007 R_386_JUMP_SLOT        00000000   pthread_create
-00003fa8  00001107 R_386_JUMP_SLOT        00000000   chmod
-00003fac  00001307 R_386_JUMP_SLOT        00000000   mkdir
-00003fb0  00001507 R_386_JUMP_SLOT        00000000   setsid
-00003fb4  00001707 R_386_JUMP_SLOT        00000000   umask
-00003fb8  00001807 R_386_JUMP_SLOT        00000000   stat
-00003fbc  00001907 R_386_JUMP_SLOT        00000000   fopen
-00003fc0  00001a07 R_386_JUMP_SLOT        00000000   fputc
-00003fc4  00001b07 R_386_JUMP_SLOT        00000000   getc
-00003fc8  00001c07 R_386_JUMP_SLOT        00000000   fclose
-00003fcc  00001e07 R_386_JUMP_SLOT        00000000   strstr
-00003fd0  00001f07 R_386_JUMP_SLOT        00000000   fgets
-00003fd4  00002007 R_386_JUMP_SLOT        00000000   strtok
-00003fd8  00002107 R_386_JUMP_SLOT        00000000   strtoul
-00003fdc  00002307 R_386_JUMP_SLOT        00000000   open
-00003fe0  00002407 R_386_JUMP_SLOT        00000000   fstat
-00003fe4  00002507 R_386_JUMP_SLOT        00000000   mmap
-00003fe8  00002607 R_386_JUMP_SLOT        00000000   memset
-00003fec  00002707 R_386_JUMP_SLOT        00000000   read
-00003ff0  00002807 R_386_JUMP_SLOT        00000000   close
-00003ff4  00002907 R_386_JUMP_SLOT        00000000   strcmp
-00003ff8  00002a07 R_386_JUMP_SLOT        00000000   munmap
-00003ffc  00002b07 R_386_JUMP_SLOT        00000000   dlsym
+00004f60  00000107 R_386_JUMP_SLOT        00000000   __libc_init
+00004f64  00000207 R_386_JUMP_SLOT        00000000   __cxa_atexit
+00004f68  00000307 R_386_JUMP_SLOT        00000000   __stack_chk_fail
+00004f6c  00000507 R_386_JUMP_SLOT        00000000   __system_property_get
+00004f70  00000607 R_386_JUMP_SLOT        00000000   atoi
+00004f74  00000707 R_386_JUMP_SLOT        00000000   printf
+00004f78  00000807 R_386_JUMP_SLOT        00000000   __android_log_print
+00004f7c  00000907 R_386_JUMP_SLOT        00000000   ptrace
+00004f80  00000a07 R_386_JUMP_SLOT        00000000   memcpy
+00004f84  00000b07 R_386_JUMP_SLOT        00000000   strlen
+00004f88  00000c07 R_386_JUMP_SLOT        00000000   perror
+00004f8c  00000d07 R_386_JUMP_SLOT        00000000   waitpid
+00004f90  00000e07 R_386_JUMP_SLOT        00000000   snprintf
+00004f94  00000f07 R_386_JUMP_SLOT        00000000   fopen
+00004f98  00001007 R_386_JUMP_SLOT        00000000   strstr
+00004f9c  00001107 R_386_JUMP_SLOT        00000000   fgets
+00004fa0  00001207 R_386_JUMP_SLOT        00000000   fclose
+00004fa4  00001307 R_386_JUMP_SLOT        00000000   strtok
+00004fa8  00001407 R_386_JUMP_SLOT        00000000   strtoul
+00004fac  00001507 R_386_JUMP_SLOT        00000000   open
+00004fb0  00001607 R_386_JUMP_SLOT        00000000   fstat
+00004fb4  00001707 R_386_JUMP_SLOT        00000000   malloc
+00004fb8  00001807 R_386_JUMP_SLOT        00000000   memset
+00004fbc  00001907 R_386_JUMP_SLOT        00000000   read
+00004fc0  00001a07 R_386_JUMP_SLOT        00000000   close
+00004fc4  00001b07 R_386_JUMP_SLOT        00000000   strcmp
+00004fc8  00001c07 R_386_JUMP_SLOT        00000000   free
+00004fcc  00001e07 R_386_JUMP_SLOT        00000000   fprintf
+00004fd0  00001f07 R_386_JUMP_SLOT        00000000   dlopen
+00004fd4  00002007 R_386_JUMP_SLOT        00000000   dlsym
+00004fd8  00002107 R_386_JUMP_SLOT        00000000   opendir
+00004fdc  00002207 R_386_JUMP_SLOT        00000000   readdir
+00004fe0  00002307 R_386_JUMP_SLOT        00000000   closedir
+00004fe4  00002407 R_386_JUMP_SLOT        00000000   sprintf
+00004fe8  00002507 R_386_JUMP_SLOT        00000000   fwrite
+00004fec  00002607 R_386_JUMP_SLOT        00000000   readlink
+00004ff0  00002707 R_386_JUMP_SLOT        00000000   lstat
+00004ff4  00002807 R_386_JUMP_SLOT        00000000   getopt_long
+00004ff8  00002a07 R_386_JUMP_SLOT        00000000   fputc
+00004ffc  00002b07 R_386_JUMP_SLOT        00000000   puts
```

#### readelf --wide --dynamic {}

```diff
@@ -1,30 +1,31 @@
 
-Dynamic section at offset 0x2e68 contains 27 entries:
+Dynamic section at offset 0x3e2c contains 28 entries:
   Tag        Type                         Name/Value
- 0x00000003 (PLTGOT)                     0x3f70
- 0x00000002 (PLTRELSZ)                   264 (bytes)
- 0x00000017 (JMPREL)                     0x7ac
+ 0x00000003 (PLTGOT)                     0x4f54
+ 0x00000002 (PLTRELSZ)                   320 (bytes)
+ 0x00000017 (JMPREL)                     0x7a8
  0x00000014 (PLTREL)                     REL
- 0x00000011 (REL)                        0x78c
- 0x00000012 (RELSZ)                      32 (bytes)
+ 0x00000011 (REL)                        0x740
+ 0x00000012 (RELSZ)                      104 (bytes)
  0x00000013 (RELENT)                     8 (bytes)
- 0x6ffffffa (RELCOUNT)                   3
- 0x00000006 (SYMTAB)                     0x114
+ 0x6ffffffa (RELCOUNT)                   9
+ 0x00000015 (DEBUG)                      0x0
+ 0x00000006 (SYMTAB)                     0x148
  0x0000000b (SYMENT)                     16 (bytes)
- 0x00000005 (STRTAB)                     0x404
- 0x0000000a (STRSZ)                      559 (bytes)
- 0x00000004 (HASH)                       0x634
+ 0x00000005 (STRTAB)                     0x438
+ 0x0000000a (STRSZ)                      432 (bytes)
+ 0x00000004 (HASH)                       0x5e8
  0x00000001 (NEEDED)                     Shared library: [liblog.so]
  0x00000001 (NEEDED)                     Shared library: [libstdc++.so]
  0x00000001 (NEEDED)                     Shared library: [libm.so]
  0x00000001 (NEEDED)                     Shared library: [libc.so]
  0x00000001 (NEEDED)                     Shared library: [libdl.so]
- 0x0000000e (SONAME)                     Library soname: [libdexloader.so]
- 0x0000001a (FINI_ARRAY)                 0x3e5c
+ 0x0000001a (FINI_ARRAY)                 0x4e14
  0x0000001c (FINI_ARRAYSZ)               8 (bytes)
- 0x00000019 (INIT_ARRAY)                 0x3e64
- 0x0000001b (INIT_ARRAYSZ)               4 (bytes)
- 0x00000010 (SYMBOLIC)                   0x0
- 0x0000001e (FLAGS)                      SYMBOLIC BIND_NOW
+ 0x00000019 (INIT_ARRAY)                 0x4e1c
+ 0x0000001b (INIT_ARRAYSZ)               8 (bytes)
+ 0x00000020 (PREINIT_ARRAY)              0x4e24
+ 0x00000021 (PREINIT_ARRAYSZ)            8 (bytes)
+ 0x0000001e (FLAGS)                      BIND_NOW
  0x6ffffffb (FLAGS_1)                    Flags: NOW
  0x00000000 (NULL)                       0x0
```

#### readelf --wide --debug-dump=frames {}

```diff
@@ -9,413 +9,851 @@
   Return address column: 8
   Augmentation data:     1b
   DW_CFA_def_cfa: r4 (esp) ofs 4
   DW_CFA_offset: r8 (eip) at cfa-4
   DW_CFA_nop
   DW_CFA_nop
 
-00000018 00000014 0000001c FDE cie=00000000 pc=00000b10..00000b23
-  DW_CFA_advance_loc: 4 to 00000b14
+00000018 00000014 0000001c FDE cie=00000000 pc=00001070..00001083
+  DW_CFA_advance_loc: 4 to 00001074
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 14 to 00000b22
+  DW_CFA_advance_loc: 14 to 00001082
   DW_CFA_def_cfa_offset: 4
   DW_CFA_nop
 
-00000030 0000001c 00000034 FDE cie=00000000 pc=00000ae0..00000b04
-  DW_CFA_advance_loc: 1 to 00000ae1
+00000030 00000018 00000034 FDE cie=00000000 pc=00001090..000010e9
+  DW_CFA_advance_loc: 1 to 00001091
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_offset: r3 (ebx) at cfa-8
-  DW_CFA_advance_loc: 15 to 00000af0
-  DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 18 to 00000b02
-  DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 1 to 00000b03
-  DW_CFA_restore: r3 (ebx)
-  DW_CFA_def_cfa_offset: 4
+  DW_CFA_offset: r5 (ebp) at cfa-8
+  DW_CFA_advance_loc: 2 to 00001093
+  DW_CFA_def_cfa_register: r5 (ebp)
+  DW_CFA_advance_loc: 1 to 00001094
+  DW_CFA_offset: r3 (ebx) at cfa-12
 
-00000050 0000001c 00000054 FDE cie=00000000 pc=00000b30..00000b66
-  DW_CFA_advance_loc: 1 to 00000b31
+0000004c 0000001c 00000050 FDE cie=00000000 pc=000010f0..00001126
+  DW_CFA_advance_loc: 1 to 000010f1
   DW_CFA_def_cfa_offset: 8
   DW_CFA_offset: r3 (ebx) at cfa-8
-  DW_CFA_advance_loc: 15 to 00000b40
+  DW_CFA_advance_loc: 15 to 00001100
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 36 to 00000b64
+  DW_CFA_advance_loc: 36 to 00001124
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 1 to 00000b65
+  DW_CFA_advance_loc: 1 to 00001125
   DW_CFA_restore: r3 (ebx)
   DW_CFA_def_cfa_offset: 4
 
-00000070 0000001c 00000074 FDE cie=00000000 pc=00000b70..00000b8b
-  DW_CFA_advance_loc: 1 to 00000b71
+0000006c 0000001c 00000070 FDE cie=00000000 pc=00001130..0000114b
+  DW_CFA_advance_loc: 1 to 00001131
   DW_CFA_def_cfa_offset: 8
   DW_CFA_offset: r3 (ebx) at cfa-8
-  DW_CFA_advance_loc: 15 to 00000b80
+  DW_CFA_advance_loc: 15 to 00001140
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 9 to 00000b89
+  DW_CFA_advance_loc: 9 to 00001149
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 1 to 00000b8a
+  DW_CFA_advance_loc: 1 to 0000114a
   DW_CFA_restore: r3 (ebx)
   DW_CFA_def_cfa_offset: 4
 
-00000090 00000010 00000094 FDE cie=00000000 pc=00000b90..00000b94
+0000008c 00000010 00000090 FDE cie=00000000 pc=0000114b..0000114f
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000000a4 00000068 000000a8 FDE cie=00000000 pc=00000ba0..00000ef5
-  DW_CFA_advance_loc: 1 to 00000ba1
+000000a0 00000034 000000a4 FDE cie=00000000 pc=00001150..00001206
+  DW_CFA_advance_loc: 1 to 00001151
+  DW_CFA_def_cfa_offset: 8
+  DW_CFA_offset: r7 (edi) at cfa-8
+  DW_CFA_advance_loc: 1 to 00001152
+  DW_CFA_def_cfa_offset: 12
+  DW_CFA_offset: r6 (esi) at cfa-12
+  DW_CFA_advance_loc: 1 to 00001153
+  DW_CFA_def_cfa_offset: 16
+  DW_CFA_offset: r3 (ebx) at cfa-16
+  DW_CFA_advance_loc: 15 to 00001162
+  DW_CFA_def_cfa_offset: 48
+  DW_CFA_advance_loc1: 155 to 000011fd
+  DW_CFA_remember_state
+  DW_CFA_def_cfa_offset: 16
+  DW_CFA_advance_loc: 1 to 000011fe
+  DW_CFA_restore: r3 (ebx)
+  DW_CFA_def_cfa_offset: 12
+  DW_CFA_advance_loc: 1 to 000011ff
+  DW_CFA_restore: r6 (esi)
+  DW_CFA_def_cfa_offset: 8
+  DW_CFA_advance_loc: 1 to 00001200
+  DW_CFA_restore: r7 (edi)
+  DW_CFA_def_cfa_offset: 4
+  DW_CFA_advance_loc: 1 to 00001201
+  DW_CFA_restore_state
+  DW_CFA_nop
+  DW_CFA_nop
+
+000000d8 00000038 000000dc FDE cie=00000000 pc=00001210..000012e8
+  DW_CFA_advance_loc: 1 to 00001211
   DW_CFA_def_cfa_offset: 8
   DW_CFA_offset: r5 (ebp) at cfa-8
-  DW_CFA_advance_loc: 1 to 00000ba2
+  DW_CFA_advance_loc: 1 to 00001212
   DW_CFA_def_cfa_offset: 12
   DW_CFA_offset: r7 (edi) at cfa-12
-  DW_CFA_advance_loc: 1 to 00000ba3
+  DW_CFA_advance_loc: 1 to 00001213
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (esi) at cfa-16
-  DW_CFA_advance_loc: 1 to 00000ba4
+  DW_CFA_advance_loc: 1 to 00001214
   DW_CFA_def_cfa_offset: 20
   DW_CFA_offset: r3 (ebx) at cfa-20
-  DW_CFA_advance_loc: 15 to 00000bb3
-  DW_CFA_def_cfa_offset: 96
-  DW_CFA_advance_loc2: 629 to 00000e28
-  DW_CFA_remember_state
+  DW_CFA_advance_loc: 15 to 00001223
+  DW_CFA_def_cfa_offset: 80
+  DW_CFA_advance_loc1: 190 to 000012e1
   DW_CFA_def_cfa_offset: 20
-  DW_CFA_advance_loc: 3 to 00000e2b
+  DW_CFA_advance_loc: 3 to 000012e4
   DW_CFA_restore: r3 (ebx)
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 1 to 00000e2c
+  DW_CFA_advance_loc: 1 to 000012e5
   DW_CFA_restore: r6 (esi)
   DW_CFA_def_cfa_offset: 12
-  DW_CFA_advance_loc: 1 to 00000e2d
+  DW_CFA_advance_loc: 1 to 000012e6
   DW_CFA_restore: r7 (edi)
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 1 to 00000e2e
+  DW_CFA_advance_loc: 1 to 000012e7
   DW_CFA_restore: r5 (ebp)
   DW_CFA_def_cfa_offset: 4
-  DW_CFA_advance_loc: 2 to 00000e30
-  DW_CFA_restore_state
-  DW_CFA_advance_loc1: 149 to 00000ec5
+
+00000114 00000050 00000118 FDE cie=00000000 pc=000012f0..0000140d
+  DW_CFA_advance_loc: 1 to 000012f1
+  DW_CFA_def_cfa_offset: 8
+  DW_CFA_offset: r5 (ebp) at cfa-8
+  DW_CFA_advance_loc: 1 to 000012f2
+  DW_CFA_def_cfa_offset: 12
+  DW_CFA_offset: r7 (edi) at cfa-12
+  DW_CFA_advance_loc: 1 to 000012f3
+  DW_CFA_def_cfa_offset: 16
+  DW_CFA_offset: r6 (esi) at cfa-16
+  DW_CFA_advance_loc: 1 to 000012f4
+  DW_CFA_def_cfa_offset: 20
+  DW_CFA_offset: r3 (ebx) at cfa-20
+  DW_CFA_advance_loc: 15 to 00001303
+  DW_CFA_def_cfa_offset: 80
+  DW_CFA_advance_loc1: 140 to 0000138f
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 20
-  DW_CFA_advance_loc: 3 to 00000ec8
+  DW_CFA_advance_loc: 3 to 00001392
   DW_CFA_restore: r3 (ebx)
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 1 to 00000ec9
+  DW_CFA_advance_loc: 1 to 00001393
   DW_CFA_restore: r6 (esi)
   DW_CFA_def_cfa_offset: 12
-  DW_CFA_advance_loc: 1 to 00000eca
+  DW_CFA_advance_loc: 1 to 00001394
   DW_CFA_restore: r7 (edi)
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 1 to 00000ecb
+  DW_CFA_advance_loc: 1 to 00001395
   DW_CFA_restore: r5 (ebp)
   DW_CFA_def_cfa_offset: 4
-  DW_CFA_advance_loc: 5 to 00000ed0
+  DW_CFA_advance_loc: 3 to 00001398
   DW_CFA_restore_state
-  DW_CFA_advance_loc: 30 to 00000eee
+  DW_CFA_advance_loc1: 110 to 00001406
   DW_CFA_def_cfa_offset: 20
-  DW_CFA_advance_loc: 3 to 00000ef1
+  DW_CFA_advance_loc: 3 to 00001409
   DW_CFA_restore: r3 (ebx)
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 1 to 00000ef2
+  DW_CFA_advance_loc: 1 to 0000140a
   DW_CFA_restore: r6 (esi)
   DW_CFA_def_cfa_offset: 12
-  DW_CFA_advance_loc: 1 to 00000ef3
+  DW_CFA_advance_loc: 1 to 0000140b
   DW_CFA_restore: r7 (edi)
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 1 to 00000ef4
+  DW_CFA_advance_loc: 1 to 0000140c
   DW_CFA_restore: r5 (ebp)
   DW_CFA_def_cfa_offset: 4
   DW_CFA_nop
-  DW_CFA_nop
 
-00000110 00000040 00000114 FDE cie=00000000 pc=00000f00..000012de
-  DW_CFA_advance_loc: 1 to 00000f01
+00000168 00000038 0000016c FDE cie=00000000 pc=00001410..000014a7
+  DW_CFA_advance_loc: 1 to 00001411
   DW_CFA_def_cfa_offset: 8
   DW_CFA_offset: r5 (ebp) at cfa-8
-  DW_CFA_advance_loc: 1 to 00000f02
+  DW_CFA_advance_loc: 1 to 00001412
   DW_CFA_def_cfa_offset: 12
   DW_CFA_offset: r7 (edi) at cfa-12
-  DW_CFA_advance_loc: 1 to 00000f03
+  DW_CFA_advance_loc: 1 to 00001413
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (esi) at cfa-16
-  DW_CFA_advance_loc: 1 to 00000f04
+  DW_CFA_advance_loc: 1 to 00001414
   DW_CFA_def_cfa_offset: 20
   DW_CFA_offset: r3 (ebx) at cfa-20
-  DW_CFA_advance_loc: 18 to 00000f16
-  DW_CFA_def_cfa_offset: 896
-  DW_CFA_advance_loc2: 812 to 00001242
-  DW_CFA_remember_state
+  DW_CFA_advance_loc: 15 to 00001423
+  DW_CFA_def_cfa_offset: 64
+  DW_CFA_advance_loc1: 127 to 000014a2
   DW_CFA_def_cfa_offset: 20
-  DW_CFA_advance_loc: 1 to 00001243
+  DW_CFA_advance_loc: 1 to 000014a3
   DW_CFA_restore: r3 (ebx)
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 1 to 00001244
+  DW_CFA_advance_loc: 1 to 000014a4
   DW_CFA_restore: r6 (esi)
   DW_CFA_def_cfa_offset: 12
-  DW_CFA_advance_loc: 1 to 00001245
+  DW_CFA_advance_loc: 1 to 000014a5
   DW_CFA_restore: r7 (edi)
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 1 to 00001246
+  DW_CFA_advance_loc: 1 to 000014a6
   DW_CFA_restore: r5 (ebp)
   DW_CFA_def_cfa_offset: 4
-  DW_CFA_advance_loc: 2 to 00001248
-  DW_CFA_restore_state
-  DW_CFA_nop
-  DW_CFA_nop
-  DW_CFA_nop
 
-00000154 0000001c 00000158 FDE cie=00000000 pc=000012e0..000012fb
-  DW_CFA_advance_loc: 1 to 000012e1
+000001a4 00000020 000001a8 FDE cie=00000000 pc=000014b0..00001505
+  DW_CFA_advance_loc: 1 to 000014b1
   DW_CFA_def_cfa_offset: 8
   DW_CFA_offset: r3 (ebx) at cfa-8
-  DW_CFA_advance_loc: 15 to 000012f0
-  DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 9 to 000012f9
+  DW_CFA_advance_loc: 15 to 000014c0
+  DW_CFA_def_cfa_offset: 32
+  DW_CFA_advance_loc: 46 to 000014ee
+  DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 1 to 000012fa
+  DW_CFA_advance_loc: 1 to 000014ef
   DW_CFA_restore: r3 (ebx)
   DW_CFA_def_cfa_offset: 4
+  DW_CFA_advance_loc: 1 to 000014f0
+  DW_CFA_restore_state
+  DW_CFA_nop
 
-00000174 0000001c 00000178 FDE cie=00000000 pc=00001300..00001325
-  DW_CFA_advance_loc: 1 to 00001301
+000001c8 00000020 000001cc FDE cie=00000000 pc=00001510..00001565
+  DW_CFA_advance_loc: 1 to 00001511
   DW_CFA_def_cfa_offset: 8
   DW_CFA_offset: r3 (ebx) at cfa-8
-  DW_CFA_advance_loc: 15 to 00001310
+  DW_CFA_advance_loc: 15 to 00001520
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 17 to 00001321
+  DW_CFA_advance_loc: 46 to 0000154e
+  DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 3 to 00001324
+  DW_CFA_advance_loc: 1 to 0000154f
   DW_CFA_restore: r3 (ebx)
   DW_CFA_def_cfa_offset: 4
+  DW_CFA_advance_loc: 1 to 00001550
+  DW_CFA_restore_state
+  DW_CFA_nop
+
+000001ec 00000030 000001f0 FDE cie=00000000 pc=00001570..000015cc
+  DW_CFA_advance_loc: 1 to 00001571
+  DW_CFA_def_cfa_offset: 8
+  DW_CFA_offset: r5 (ebp) at cfa-8
+  DW_CFA_advance_loc: 1 to 00001572
+  DW_CFA_def_cfa_offset: 12
+  DW_CFA_offset: r7 (edi) at cfa-12
+  DW_CFA_advance_loc: 1 to 00001573
+  DW_CFA_def_cfa_offset: 16
+  DW_CFA_offset: r6 (esi) at cfa-16
+  DW_CFA_advance_loc: 4 to 00001577
+  DW_CFA_def_cfa_offset: 112
+  DW_CFA_advance_loc1: 79 to 000015c6
+  DW_CFA_def_cfa_offset: 16
+  DW_CFA_advance_loc: 3 to 000015c9
+  DW_CFA_restore: r6 (esi)
+  DW_CFA_def_cfa_offset: 12
+  DW_CFA_advance_loc: 1 to 000015ca
+  DW_CFA_restore: r7 (edi)
+  DW_CFA_def_cfa_offset: 8
+  DW_CFA_advance_loc: 1 to 000015cb
+  DW_CFA_restore: r5 (ebp)
+  DW_CFA_def_cfa_offset: 4
+  DW_CFA_nop
 
-00000194 00000020 00000198 FDE cie=00000000 pc=00001330..0000136d
-  DW_CFA_advance_loc: 1 to 00001331
+00000220 00000020 00000224 FDE cie=00000000 pc=000015d0..00001625
+  DW_CFA_advance_loc: 1 to 000015d1
   DW_CFA_def_cfa_offset: 8
   DW_CFA_offset: r3 (ebx) at cfa-8
-  DW_CFA_advance_loc: 15 to 00001340
-  DW_CFA_def_cfa_offset: 128
-  DW_CFA_advance_loc: 41 to 00001369
+  DW_CFA_advance_loc: 15 to 000015e0
+  DW_CFA_def_cfa_offset: 32
+  DW_CFA_advance_loc: 46 to 0000160e
+  DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 1 to 0000136a
+  DW_CFA_advance_loc: 1 to 0000160f
   DW_CFA_restore: r3 (ebx)
   DW_CFA_def_cfa_offset: 4
+  DW_CFA_advance_loc: 1 to 00001610
+  DW_CFA_restore_state
   DW_CFA_nop
+
+00000244 00000050 00000248 FDE cie=00000000 pc=00001630..00001776
+  DW_CFA_advance_loc: 1 to 00001631
+  DW_CFA_def_cfa_offset: 8
+  DW_CFA_offset: r5 (ebp) at cfa-8
+  DW_CFA_advance_loc: 3 to 00001634
+  DW_CFA_def_cfa_offset: 12
+  DW_CFA_offset: r7 (edi) at cfa-12
+  DW_CFA_advance_loc: 1 to 00001635
+  DW_CFA_def_cfa_offset: 16
+  DW_CFA_offset: r6 (esi) at cfa-16
+  DW_CFA_advance_loc: 1 to 00001636
+  DW_CFA_def_cfa_offset: 20
+  DW_CFA_offset: r3 (ebx) at cfa-20
+  DW_CFA_advance_loc: 15 to 00001645
+  DW_CFA_def_cfa_offset: 80
+  DW_CFA_advance_loc2: 279 to 0000175c
+  DW_CFA_remember_state
+  DW_CFA_def_cfa_offset: 20
+  DW_CFA_advance_loc: 1 to 0000175d
+  DW_CFA_restore: r3 (ebx)
+  DW_CFA_def_cfa_offset: 16
+  DW_CFA_advance_loc: 1 to 0000175e
+  DW_CFA_restore: r6 (esi)
+  DW_CFA_def_cfa_offset: 12
+  DW_CFA_advance_loc: 1 to 0000175f
+  DW_CFA_restore: r7 (edi)
+  DW_CFA_def_cfa_offset: 8
+  DW_CFA_advance_loc: 1 to 00001760
+  DW_CFA_restore: r5 (ebp)
+  DW_CFA_def_cfa_offset: 4
+  DW_CFA_advance_loc: 8 to 00001768
+  DW_CFA_restore_state
+  DW_CFA_advance_loc: 4 to 0000176c
+  DW_CFA_def_cfa_offset: 20
+  DW_CFA_advance_loc: 6 to 00001772
+  DW_CFA_restore: r3 (ebx)
+  DW_CFA_def_cfa_offset: 16
+  DW_CFA_advance_loc: 1 to 00001773
+  DW_CFA_restore: r6 (esi)
+  DW_CFA_def_cfa_offset: 12
+  DW_CFA_advance_loc: 1 to 00001774
+  DW_CFA_restore: r7 (edi)
+  DW_CFA_def_cfa_offset: 8
+  DW_CFA_advance_loc: 1 to 00001775
+  DW_CFA_restore: r5 (ebp)
+  DW_CFA_def_cfa_offset: 4
   DW_CFA_nop
+
+00000298 00000020 0000029c FDE cie=00000000 pc=00001780..000017d5
+  DW_CFA_advance_loc: 1 to 00001781
+  DW_CFA_def_cfa_offset: 8
+  DW_CFA_offset: r3 (ebx) at cfa-8
+  DW_CFA_advance_loc: 15 to 00001790
+  DW_CFA_def_cfa_offset: 32
+  DW_CFA_advance_loc: 46 to 000017be
+  DW_CFA_remember_state
+  DW_CFA_def_cfa_offset: 8
+  DW_CFA_advance_loc: 1 to 000017bf
+  DW_CFA_restore: r3 (ebx)
+  DW_CFA_def_cfa_offset: 4
+  DW_CFA_advance_loc: 1 to 000017c0
+  DW_CFA_restore_state
   DW_CFA_nop
 
-000001b8 0000003c 000001bc FDE cie=00000000 pc=00001370..00001453
-  DW_CFA_advance_loc: 1 to 00001371
+000002bc 0000003c 000002c0 FDE cie=00000000 pc=000017e0..000019ed
+  DW_CFA_advance_loc: 1 to 000017e1
   DW_CFA_def_cfa_offset: 8
   DW_CFA_offset: r5 (ebp) at cfa-8
-  DW_CFA_advance_loc: 1 to 00001372
+  DW_CFA_advance_loc: 1 to 000017e2
   DW_CFA_def_cfa_offset: 12
   DW_CFA_offset: r7 (edi) at cfa-12
-  DW_CFA_advance_loc: 1 to 00001373
+  DW_CFA_advance_loc: 1 to 000017e3
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (esi) at cfa-16
-  DW_CFA_advance_loc: 1 to 00001374
+  DW_CFA_advance_loc: 1 to 000017e4
   DW_CFA_def_cfa_offset: 20
   DW_CFA_offset: r3 (ebx) at cfa-20
-  DW_CFA_advance_loc: 15 to 00001383
+  DW_CFA_advance_loc: 15 to 000017f3
   DW_CFA_def_cfa_offset: 64
-  DW_CFA_advance_loc1: 156 to 0000141f
+  DW_CFA_advance_loc2: 441 to 000019ac
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 20
-  DW_CFA_advance_loc: 1 to 00001420
+  DW_CFA_advance_loc: 1 to 000019ad
   DW_CFA_restore: r3 (ebx)
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 1 to 00001421
+  DW_CFA_advance_loc: 1 to 000019ae
   DW_CFA_restore: r6 (esi)
   DW_CFA_def_cfa_offset: 12
-  DW_CFA_advance_loc: 1 to 00001422
+  DW_CFA_advance_loc: 1 to 000019af
   DW_CFA_restore: r7 (edi)
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 1 to 00001423
+  DW_CFA_advance_loc: 1 to 000019b0
   DW_CFA_restore: r5 (ebp)
   DW_CFA_def_cfa_offset: 4
-  DW_CFA_advance_loc: 1 to 00001424
+  DW_CFA_advance_loc: 8 to 000019b8
   DW_CFA_restore_state
-  DW_CFA_nop
 
-000001f8 0000003c 000001fc FDE cie=00000000 pc=00001460..00001555
-  DW_CFA_advance_loc: 1 to 00001461
+000002fc 0000003c 00000300 FDE cie=00000000 pc=000019f0..00001b35
+  DW_CFA_advance_loc: 1 to 000019f1
   DW_CFA_def_cfa_offset: 8
   DW_CFA_offset: r5 (ebp) at cfa-8
-  DW_CFA_advance_loc: 1 to 00001462
+  DW_CFA_advance_loc: 1 to 000019f2
   DW_CFA_def_cfa_offset: 12
   DW_CFA_offset: r7 (edi) at cfa-12
-  DW_CFA_advance_loc: 1 to 00001463
+  DW_CFA_advance_loc: 1 to 000019f3
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (esi) at cfa-16
-  DW_CFA_advance_loc: 1 to 00001464
+  DW_CFA_advance_loc: 1 to 000019f4
   DW_CFA_def_cfa_offset: 20
   DW_CFA_offset: r3 (ebx) at cfa-20
-  DW_CFA_advance_loc: 18 to 00001476
-  DW_CFA_def_cfa_offset: 1088
-  DW_CFA_advance_loc1: 144 to 00001506
+  DW_CFA_advance_loc: 18 to 00001a06
+  DW_CFA_def_cfa_offset: 1120
+  DW_CFA_advance_loc1: 184 to 00001abe
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 20
-  DW_CFA_advance_loc: 1 to 00001507
+  DW_CFA_advance_loc: 1 to 00001abf
   DW_CFA_restore: r3 (ebx)
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 1 to 00001508
+  DW_CFA_advance_loc: 1 to 00001ac0
   DW_CFA_restore: r6 (esi)
   DW_CFA_def_cfa_offset: 12
-  DW_CFA_advance_loc: 1 to 00001509
+  DW_CFA_advance_loc: 1 to 00001ac1
   DW_CFA_restore: r7 (edi)
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 1 to 0000150a
+  DW_CFA_advance_loc: 1 to 00001ac2
   DW_CFA_restore: r5 (ebp)
   DW_CFA_def_cfa_offset: 4
-  DW_CFA_advance_loc: 6 to 00001510
+  DW_CFA_advance_loc: 6 to 00001ac8
   DW_CFA_restore_state
 
-00000238 00000080 0000023c FDE cie=00000000 pc=00001560..00001906
-  DW_CFA_advance_loc: 1 to 00001561
+0000033c 00000028 00000340 FDE cie=00000000 pc=00001b40..00001b79
+  DW_CFA_advance_loc: 1 to 00001b41
+  DW_CFA_def_cfa_offset: 8
+  DW_CFA_offset: r7 (edi) at cfa-8
+  DW_CFA_advance_loc: 1 to 00001b42
+  DW_CFA_def_cfa_offset: 12
+  DW_CFA_offset: r6 (esi) at cfa-12
+  DW_CFA_advance_loc: 4 to 00001b46
+  DW_CFA_def_cfa_offset: 32
+  DW_CFA_advance_loc: 46 to 00001b74
+  DW_CFA_def_cfa_offset: 12
+  DW_CFA_advance_loc: 1 to 00001b75
+  DW_CFA_restore: r6 (esi)
+  DW_CFA_def_cfa_offset: 8
+  DW_CFA_advance_loc: 3 to 00001b78
+  DW_CFA_restore: r7 (edi)
+  DW_CFA_def_cfa_offset: 4
+  DW_CFA_nop
+  DW_CFA_nop
+  DW_CFA_nop
+
+00000368 00000080 0000036c FDE cie=00000000 pc=00001b80..00001e4f
+  DW_CFA_advance_loc: 1 to 00001b81
   DW_CFA_def_cfa_offset: 8
   DW_CFA_offset: r5 (ebp) at cfa-8
-  DW_CFA_advance_loc: 1 to 00001562
+  DW_CFA_advance_loc: 1 to 00001b82
   DW_CFA_def_cfa_offset: 12
   DW_CFA_offset: r7 (edi) at cfa-12
-  DW_CFA_advance_loc: 1 to 00001563
+  DW_CFA_advance_loc: 1 to 00001b83
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (esi) at cfa-16
-  DW_CFA_advance_loc: 1 to 00001564
+  DW_CFA_advance_loc: 1 to 00001b84
   DW_CFA_def_cfa_offset: 20
   DW_CFA_offset: r3 (ebx) at cfa-20
-  DW_CFA_advance_loc: 18 to 00001576
-  DW_CFA_def_cfa_offset: 192
-  DW_CFA_advance_loc2: 578 to 000017b8
+  DW_CFA_advance_loc: 18 to 00001b96
+  DW_CFA_def_cfa_offset: 176
+  DW_CFA_advance_loc2: 442 to 00001d50
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 20
-  DW_CFA_advance_loc: 1 to 000017b9
+  DW_CFA_advance_loc: 1 to 00001d51
   DW_CFA_restore: r3 (ebx)
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 1 to 000017ba
+  DW_CFA_advance_loc: 1 to 00001d52
   DW_CFA_restore: r6 (esi)
   DW_CFA_def_cfa_offset: 12
-  DW_CFA_advance_loc: 1 to 000017bb
+  DW_CFA_advance_loc: 1 to 00001d53
   DW_CFA_restore: r7 (edi)
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 1 to 000017bc
+  DW_CFA_advance_loc: 1 to 00001d54
   DW_CFA_restore: r5 (ebp)
   DW_CFA_def_cfa_offset: 4
-  DW_CFA_advance_loc: 4 to 000017c0
+  DW_CFA_advance_loc: 4 to 00001d58
   DW_CFA_restore_state
-  DW_CFA_advance_loc: 49 to 000017f1
+  DW_CFA_advance_loc1: 144 to 00001de8
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 20
-  DW_CFA_advance_loc: 1 to 000017f2
+  DW_CFA_advance_loc: 3 to 00001deb
   DW_CFA_restore: r3 (ebx)
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 1 to 000017f3
+  DW_CFA_advance_loc: 1 to 00001dec
   DW_CFA_restore: r6 (esi)
   DW_CFA_def_cfa_offset: 12
-  DW_CFA_advance_loc: 1 to 000017f4
+  DW_CFA_advance_loc: 1 to 00001ded
   DW_CFA_restore: r7 (edi)
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 1 to 000017f5
+  DW_CFA_advance_loc: 1 to 00001dee
   DW_CFA_restore: r5 (ebp)
   DW_CFA_def_cfa_offset: 4
-  DW_CFA_advance_loc: 3 to 000017f8
+  DW_CFA_advance_loc: 1 to 00001def
   DW_CFA_restore_state
-  DW_CFA_advance_loc1: 150 to 0000188e
+  DW_CFA_advance_loc: 40 to 00001e17
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 20
-  DW_CFA_advance_loc: 3 to 00001891
+  DW_CFA_advance_loc: 3 to 00001e1a
   DW_CFA_restore: r3 (ebx)
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 1 to 00001892
+  DW_CFA_advance_loc: 1 to 00001e1b
   DW_CFA_restore: r6 (esi)
   DW_CFA_def_cfa_offset: 12
-  DW_CFA_advance_loc: 1 to 00001893
+  DW_CFA_advance_loc: 1 to 00001e1c
   DW_CFA_restore: r7 (edi)
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 1 to 00001894
+  DW_CFA_advance_loc: 1 to 00001e1d
   DW_CFA_restore: r5 (ebp)
   DW_CFA_def_cfa_offset: 4
-  DW_CFA_advance_loc: 4 to 00001898
+  DW_CFA_advance_loc: 1 to 00001e1e
   DW_CFA_restore_state
-  DW_CFA_advance_loc: 43 to 000018c3
+  DW_CFA_advance_loc: 19 to 00001e31
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 20
-  DW_CFA_advance_loc: 3 to 000018c6
+  DW_CFA_advance_loc: 3 to 00001e34
   DW_CFA_restore: r3 (ebx)
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 1 to 000018c7
+  DW_CFA_advance_loc: 1 to 00001e35
   DW_CFA_restore: r6 (esi)
   DW_CFA_def_cfa_offset: 12
-  DW_CFA_advance_loc: 1 to 000018c8
+  DW_CFA_advance_loc: 1 to 00001e36
   DW_CFA_restore: r7 (edi)
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 1 to 000018c9
+  DW_CFA_advance_loc: 1 to 00001e37
   DW_CFA_restore: r5 (ebp)
   DW_CFA_def_cfa_offset: 4
-  DW_CFA_advance_loc: 1 to 000018ca
+  DW_CFA_advance_loc: 1 to 00001e38
   DW_CFA_restore_state
 
-000002bc 00000054 000002c0 FDE cie=00000000 pc=00001910..00001a52
-  DW_CFA_advance_loc: 1 to 00001911
+000003ec 00000050 000003f0 FDE cie=00000000 pc=00001e50..00001f4d
+  DW_CFA_advance_loc: 1 to 00001e51
   DW_CFA_def_cfa_offset: 8
   DW_CFA_offset: r5 (ebp) at cfa-8
-  DW_CFA_advance_loc: 1 to 00001912
+  DW_CFA_advance_loc: 1 to 00001e52
   DW_CFA_def_cfa_offset: 12
   DW_CFA_offset: r7 (edi) at cfa-12
-  DW_CFA_advance_loc: 1 to 00001913
+  DW_CFA_advance_loc: 1 to 00001e53
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (esi) at cfa-16
-  DW_CFA_advance_loc: 1 to 00001914
+  DW_CFA_advance_loc: 1 to 00001e54
   DW_CFA_def_cfa_offset: 20
   DW_CFA_offset: r3 (ebx) at cfa-20
-  DW_CFA_advance_loc: 15 to 00001923
+  DW_CFA_advance_loc: 15 to 00001e63
   DW_CFA_def_cfa_offset: 64
-  DW_CFA_advance_loc1: 70 to 00001969
+  DW_CFA_advance_loc1: 126 to 00001ee1
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 20
-  DW_CFA_advance_loc: 1 to 0000196a
+  DW_CFA_advance_loc: 1 to 00001ee2
   DW_CFA_restore: r3 (ebx)
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 1 to 0000196b
+  DW_CFA_advance_loc: 1 to 00001ee3
   DW_CFA_restore: r6 (esi)
   DW_CFA_def_cfa_offset: 12
-  DW_CFA_advance_loc: 1 to 0000196c
+  DW_CFA_advance_loc: 1 to 00001ee4
   DW_CFA_restore: r7 (edi)
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 1 to 0000196d
+  DW_CFA_advance_loc: 1 to 00001ee5
   DW_CFA_restore: r5 (ebp)
   DW_CFA_def_cfa_offset: 4
-  DW_CFA_advance_loc: 3 to 00001970
+  DW_CFA_advance_loc: 3 to 00001ee8
   DW_CFA_restore_state
-  DW_CFA_advance_loc1: 134 to 000019f6
+  DW_CFA_advance_loc1: 94 to 00001f46
+  DW_CFA_def_cfa_offset: 20
+  DW_CFA_advance_loc: 3 to 00001f49
+  DW_CFA_restore: r3 (ebx)
+  DW_CFA_def_cfa_offset: 16
+  DW_CFA_advance_loc: 1 to 00001f4a
+  DW_CFA_restore: r6 (esi)
+  DW_CFA_def_cfa_offset: 12
+  DW_CFA_advance_loc: 1 to 00001f4b
+  DW_CFA_restore: r7 (edi)
+  DW_CFA_def_cfa_offset: 8
+  DW_CFA_advance_loc: 1 to 00001f4c
+  DW_CFA_restore: r5 (ebp)
+  DW_CFA_def_cfa_offset: 4
+  DW_CFA_nop
+
+00000440 0000003c 00000444 FDE cie=00000000 pc=00001f50..0000208a
+  DW_CFA_advance_loc: 1 to 00001f51
+  DW_CFA_def_cfa_offset: 8
+  DW_CFA_offset: r5 (ebp) at cfa-8
+  DW_CFA_advance_loc: 1 to 00001f52
+  DW_CFA_def_cfa_offset: 12
+  DW_CFA_offset: r7 (edi) at cfa-12
+  DW_CFA_advance_loc: 1 to 00001f53
+  DW_CFA_def_cfa_offset: 16
+  DW_CFA_offset: r6 (esi) at cfa-16
+  DW_CFA_advance_loc: 1 to 00001f54
+  DW_CFA_def_cfa_offset: 20
+  DW_CFA_offset: r3 (ebx) at cfa-20
+  DW_CFA_advance_loc: 18 to 00001f66
+  DW_CFA_def_cfa_offset: 368
+  DW_CFA_advance_loc1: 140 to 00001ff2
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 20
-  DW_CFA_advance_loc: 1 to 000019f7
+  DW_CFA_advance_loc: 1 to 00001ff3
   DW_CFA_restore: r3 (ebx)
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 1 to 000019f8
+  DW_CFA_advance_loc: 1 to 00001ff4
   DW_CFA_restore: r6 (esi)
   DW_CFA_def_cfa_offset: 12
-  DW_CFA_advance_loc: 1 to 000019f9
+  DW_CFA_advance_loc: 1 to 00001ff5
   DW_CFA_restore: r7 (edi)
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 1 to 000019fa
+  DW_CFA_advance_loc: 1 to 00001ff6
   DW_CFA_restore: r5 (ebp)
   DW_CFA_def_cfa_offset: 4
-  DW_CFA_advance_loc: 6 to 00001a00
+  DW_CFA_advance_loc: 2 to 00001ff8
   DW_CFA_restore_state
+
+00000480 0000003c 00000484 FDE cie=00000000 pc=00002090..00002260
+  DW_CFA_advance_loc: 1 to 00002091
+  DW_CFA_def_cfa_offset: 8
+  DW_CFA_offset: r5 (ebp) at cfa-8
+  DW_CFA_advance_loc: 1 to 00002092
+  DW_CFA_def_cfa_offset: 12
+  DW_CFA_offset: r7 (edi) at cfa-12
+  DW_CFA_advance_loc: 1 to 00002093
+  DW_CFA_def_cfa_offset: 16
+  DW_CFA_offset: r6 (esi) at cfa-16
+  DW_CFA_advance_loc: 1 to 00002094
+  DW_CFA_def_cfa_offset: 20
+  DW_CFA_offset: r3 (ebx) at cfa-20
+  DW_CFA_advance_loc: 15 to 000020a3
+  DW_CFA_def_cfa_offset: 112
+  DW_CFA_advance_loc2: 438 to 00002259
+  DW_CFA_def_cfa_offset: 20
+  DW_CFA_advance_loc: 3 to 0000225c
+  DW_CFA_restore: r3 (ebx)
+  DW_CFA_def_cfa_offset: 16
+  DW_CFA_advance_loc: 1 to 0000225d
+  DW_CFA_restore: r6 (esi)
+  DW_CFA_def_cfa_offset: 12
+  DW_CFA_advance_loc: 1 to 0000225e
+  DW_CFA_restore: r7 (edi)
+  DW_CFA_def_cfa_offset: 8
+  DW_CFA_advance_loc: 1 to 0000225f
+  DW_CFA_restore: r5 (ebp)
+  DW_CFA_def_cfa_offset: 4
   DW_CFA_nop
   DW_CFA_nop
+  DW_CFA_nop
+
+000004c0 0000003c 000004c4 FDE cie=00000000 pc=00002260..0000234c
+  DW_CFA_advance_loc: 1 to 00002261
+  DW_CFA_def_cfa_offset: 8
+  DW_CFA_offset: r5 (ebp) at cfa-8
+  DW_CFA_advance_loc: 1 to 00002262
+  DW_CFA_def_cfa_offset: 12
+  DW_CFA_offset: r7 (edi) at cfa-12
+  DW_CFA_advance_loc: 1 to 00002263
+  DW_CFA_def_cfa_offset: 16
+  DW_CFA_offset: r6 (esi) at cfa-16
+  DW_CFA_advance_loc: 1 to 00002264
+  DW_CFA_def_cfa_offset: 20
+  DW_CFA_offset: r3 (ebx) at cfa-20
+  DW_CFA_advance_loc: 15 to 00002273
+  DW_CFA_def_cfa_offset: 144
+  DW_CFA_advance_loc1: 212 to 00002347
+  DW_CFA_def_cfa_offset: 20
+  DW_CFA_advance_loc: 1 to 00002348
+  DW_CFA_restore: r3 (ebx)
+  DW_CFA_def_cfa_offset: 16
+  DW_CFA_advance_loc: 1 to 00002349
+  DW_CFA_restore: r6 (esi)
+  DW_CFA_def_cfa_offset: 12
+  DW_CFA_advance_loc: 1 to 0000234a
+  DW_CFA_restore: r7 (edi)
+  DW_CFA_def_cfa_offset: 8
+  DW_CFA_advance_loc: 1 to 0000234b
+  DW_CFA_restore: r5 (ebp)
+  DW_CFA_def_cfa_offset: 4
+  DW_CFA_nop
+  DW_CFA_nop
+  DW_CFA_nop
+
+00000500 0000003c 00000504 FDE cie=00000000 pc=00002350..00002447
+  DW_CFA_advance_loc: 1 to 00002351
+  DW_CFA_def_cfa_offset: 8
+  DW_CFA_offset: r5 (ebp) at cfa-8
+  DW_CFA_advance_loc: 1 to 00002352
+  DW_CFA_def_cfa_offset: 12
+  DW_CFA_offset: r7 (edi) at cfa-12
+  DW_CFA_advance_loc: 1 to 00002353
+  DW_CFA_def_cfa_offset: 16
+  DW_CFA_offset: r6 (esi) at cfa-16
+  DW_CFA_advance_loc: 1 to 00002354
+  DW_CFA_def_cfa_offset: 20
+  DW_CFA_offset: r3 (ebx) at cfa-20
+  DW_CFA_advance_loc: 15 to 00002363
+  DW_CFA_def_cfa_offset: 64
+  DW_CFA_advance_loc1: 169 to 0000240c
+  DW_CFA_remember_state
+  DW_CFA_def_cfa_offset: 20
+  DW_CFA_advance_loc: 3 to 0000240f
+  DW_CFA_restore: r3 (ebx)
+  DW_CFA_def_cfa_offset: 16
+  DW_CFA_advance_loc: 1 to 00002410
+  DW_CFA_restore: r6 (esi)
+  DW_CFA_def_cfa_offset: 12
+  DW_CFA_advance_loc: 1 to 00002411
+  DW_CFA_restore: r7 (edi)
+  DW_CFA_def_cfa_offset: 8
+  DW_CFA_advance_loc: 1 to 00002412
+  DW_CFA_restore: r5 (ebp)
+  DW_CFA_def_cfa_offset: 4
+  DW_CFA_advance_loc: 6 to 00002418
+  DW_CFA_restore_state
+  DW_CFA_nop
+
+00000540 0000003c 00000544 FDE cie=00000000 pc=00002450..0000257d
+  DW_CFA_advance_loc: 1 to 00002451
+  DW_CFA_def_cfa_offset: 8
+  DW_CFA_offset: r5 (ebp) at cfa-8
+  DW_CFA_advance_loc: 6 to 00002457
+  DW_CFA_def_cfa_offset: 12
+  DW_CFA_offset: r7 (edi) at cfa-12
+  DW_CFA_advance_loc: 1 to 00002458
+  DW_CFA_def_cfa_offset: 16
+  DW_CFA_offset: r6 (esi) at cfa-16
+  DW_CFA_advance_loc: 1 to 00002459
+  DW_CFA_def_cfa_offset: 20
+  DW_CFA_offset: r3 (ebx) at cfa-20
+  DW_CFA_advance_loc: 18 to 0000246b
+  DW_CFA_def_cfa_offset: 336
+  DW_CFA_advance_loc1: 223 to 0000254a
+  DW_CFA_remember_state
+  DW_CFA_def_cfa_offset: 20
+  DW_CFA_advance_loc: 1 to 0000254b
+  DW_CFA_restore: r3 (ebx)
+  DW_CFA_def_cfa_offset: 16
+  DW_CFA_advance_loc: 1 to 0000254c
+  DW_CFA_restore: r6 (esi)
+  DW_CFA_def_cfa_offset: 12
+  DW_CFA_advance_loc: 1 to 0000254d
+  DW_CFA_restore: r7 (edi)
+  DW_CFA_def_cfa_offset: 8
+  DW_CFA_advance_loc: 1 to 0000254e
+  DW_CFA_restore: r5 (ebp)
+  DW_CFA_def_cfa_offset: 4
+  DW_CFA_advance_loc: 2 to 00002550
+  DW_CFA_restore_state
+
+00000580 00000040 00000584 FDE cie=00000000 pc=00002580..00002c61
+  DW_CFA_advance_loc: 1 to 00002581
+  DW_CFA_def_cfa_offset: 8
+  DW_CFA_offset: r5 (ebp) at cfa-8
+  DW_CFA_advance_loc: 1 to 00002582
+  DW_CFA_def_cfa_offset: 12
+  DW_CFA_offset: r7 (edi) at cfa-12
+  DW_CFA_advance_loc: 1 to 00002583
+  DW_CFA_def_cfa_offset: 16
+  DW_CFA_offset: r6 (esi) at cfa-16
+  DW_CFA_advance_loc: 1 to 00002584
+  DW_CFA_def_cfa_offset: 20
+  DW_CFA_offset: r3 (ebx) at cfa-20
+  DW_CFA_advance_loc: 18 to 00002596
+  DW_CFA_def_cfa_offset: 256
+  DW_CFA_advance_loc2: 647 to 0000281d
+  DW_CFA_remember_state
+  DW_CFA_def_cfa_offset: 20
+  DW_CFA_advance_loc: 3 to 00002820
+  DW_CFA_restore: r3 (ebx)
+  DW_CFA_def_cfa_offset: 16
+  DW_CFA_advance_loc: 1 to 00002821
+  DW_CFA_restore: r6 (esi)
+  DW_CFA_def_cfa_offset: 12
+  DW_CFA_advance_loc: 1 to 00002822
+  DW_CFA_restore: r7 (edi)
+  DW_CFA_def_cfa_offset: 8
+  DW_CFA_advance_loc: 1 to 00002823
+  DW_CFA_restore: r5 (ebp)
+  DW_CFA_def_cfa_offset: 4
+  DW_CFA_advance_loc: 5 to 00002828
+  DW_CFA_restore_state
+  DW_CFA_nop
+  DW_CFA_nop
+  DW_CFA_nop
+
+000005c4 00000040 000005c8 FDE cie=00000000 pc=00002c70..00002cce
+  DW_CFA_advance_loc: 1 to 00002c71
+  DW_CFA_def_cfa_offset: 8
+  DW_CFA_offset: r7 (edi) at cfa-8
+  DW_CFA_advance_loc: 1 to 00002c72
+  DW_CFA_def_cfa_offset: 12
+  DW_CFA_offset: r6 (esi) at cfa-12
+  DW_CFA_advance_loc: 1 to 00002c73
+  DW_CFA_def_cfa_offset: 16
+  DW_CFA_offset: r3 (ebx) at cfa-16
+  DW_CFA_advance_loc: 15 to 00002c82
+  DW_CFA_def_cfa_offset: 32
+  DW_CFA_advance_loc: 47 to 00002cb1
+  DW_CFA_remember_state
+  DW_CFA_def_cfa_offset: 16
+  DW_CFA_advance_loc: 1 to 00002cb2
+  DW_CFA_restore: r3 (ebx)
+  DW_CFA_def_cfa_offset: 12
+  DW_CFA_advance_loc: 1 to 00002cb3
+  DW_CFA_restore: r6 (esi)
+  DW_CFA_def_cfa_offset: 8
+  DW_CFA_advance_loc: 1 to 00002cb4
+  DW_CFA_restore: r7 (edi)
+  DW_CFA_def_cfa_offset: 4
+  DW_CFA_advance_loc: 4 to 00002cb8
+  DW_CFA_restore_state
+  DW_CFA_advance_loc: 18 to 00002cca
+  DW_CFA_def_cfa_offset: 16
+  DW_CFA_advance_loc: 1 to 00002ccb
+  DW_CFA_restore: r3 (ebx)
+  DW_CFA_def_cfa_offset: 12
+  DW_CFA_advance_loc: 1 to 00002ccc
+  DW_CFA_restore: r6 (esi)
+  DW_CFA_def_cfa_offset: 8
+  DW_CFA_advance_loc: 1 to 00002ccd
+  DW_CFA_restore: r7 (edi)
+  DW_CFA_def_cfa_offset: 4
+
+00000608 00000034 0000060c FDE cie=00000000 pc=00002cd0..00002d2b
+  DW_CFA_advance_loc: 1 to 00002cd1
+  DW_CFA_def_cfa_offset: 8
+  DW_CFA_offset: r6 (esi) at cfa-8
+  DW_CFA_advance_loc: 1 to 00002cd2
+  DW_CFA_def_cfa_offset: 12
+  DW_CFA_offset: r3 (ebx) at cfa-12
+  DW_CFA_advance_loc: 15 to 00002ce1
+  DW_CFA_def_cfa_offset: 128
+  DW_CFA_advance_loc: 43 to 00002d0c
+  DW_CFA_remember_state
+  DW_CFA_def_cfa_offset: 12
+  DW_CFA_advance_loc: 1 to 00002d0d
+  DW_CFA_restore: r3 (ebx)
+  DW_CFA_def_cfa_offset: 8
+  DW_CFA_advance_loc: 1 to 00002d0e
+  DW_CFA_restore: r6 (esi)
+  DW_CFA_def_cfa_offset: 4
+  DW_CFA_advance_loc: 2 to 00002d10
+  DW_CFA_restore_state
+  DW_CFA_advance_loc: 24 to 00002d28
+  DW_CFA_def_cfa_offset: 12
+  DW_CFA_advance_loc: 1 to 00002d29
+  DW_CFA_restore: r3 (ebx)
+  DW_CFA_def_cfa_offset: 8
+  DW_CFA_advance_loc: 1 to 00002d2a
+  DW_CFA_restore: r6 (esi)
+  DW_CFA_def_cfa_offset: 4
+
+00000640 0000002c 00000644 FDE cie=00000000 pc=00000b80..00001064
+  DW_CFA_advance_loc: 1 to 00000b81
+  DW_CFA_def_cfa_offset: 8
+  DW_CFA_offset: r5 (ebp) at cfa-8
+  DW_CFA_advance_loc: 7 to 00000b88
+  DW_CFA_def_cfa_register: r5 (ebp)
+  DW_CFA_advance_loc: 3 to 00000b8b
+  DW_CFA_offset: r7 (edi) at cfa-12
+  DW_CFA_offset: r6 (esi) at cfa-16
+  DW_CFA_offset: r3 (ebx) at cfa-20
+  DW_CFA_advance_loc2: 527 to 00000d9a
+  DW_CFA_remember_state
+  DW_CFA_restore: r3 (ebx)
+  DW_CFA_advance_loc: 1 to 00000d9b
+  DW_CFA_restore: r6 (esi)
+  DW_CFA_advance_loc: 1 to 00000d9c
+  DW_CFA_restore: r7 (edi)
+  DW_CFA_advance_loc: 1 to 00000d9d
+  DW_CFA_restore: r5 (ebp)
+  DW_CFA_def_cfa: r4 (esp) ofs 4
+  DW_CFA_advance_loc: 1 to 00000d9e
+  DW_CFA_restore_state
 
-00000314 00000024 00000318 FDE cie=00000000 pc=000008c0..00000ae0
+00000670 00000024 00000674 FDE cie=00000000 pc=000008f0..00000b80
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 6 to 000008c6
+  DW_CFA_advance_loc: 6 to 000008f6
   DW_CFA_def_cfa_offset: 12
-  DW_CFA_advance_loc: 10 to 000008d0
+  DW_CFA_advance_loc: 10 to 00000900
   DW_CFA_def_cfa_expression (DW_OP_breg4 (esp): 4; DW_OP_breg8 (eip): 0; DW_OP_lit15; DW_OP_and; DW_OP_lit11; DW_OP_ge; DW_OP_lit2; DW_OP_shl; DW_OP_plus)
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-0000033c ZERO terminator
+00000698 ZERO terminator
```

#### strings --all --bytes=8 {}

```diff
@@ -1,69 +1,94 @@
-__cxa_finalize
+/system/bin/linker
+__libc_init
 __cxa_atexit
 __stack_chk_fail
-load_dex_in_thread
-__android_log_print
-load_dex
 __stack_chk_guard
-get_file_size
-get_jni_env
-pthread_create
-copyfile
-Java_com_test_androidspy_HelperUtil_nativeSetsid
-Java_com_test_androidspy_HelperUtil_nativeUmask
-get_module_base
-get_symbol_offset
+__system_property_get
+__android_log_print
+snprintf
+closedir
+readlink
+getopt_long
 __bss_start
 liblog.so
 libstdc++.so
 libdl.so
-libdexloader.so
-Enter thread
-dexloader
-Get env failed
-Current JNIEnv: %p
-java/lang/ClassLoader
-()Ljava/lang/ClassLoader;
-getSystemClassLoader
-dalvik/system/DexClassLoader
-Object dex_loader: %p
-findClass
-Class %s: %p
-Find class %s failed
-Exit thread
-Out file dir: %s
-JNIEnv: %p
-Get jvm failed: %d
-JavaVM: %p
-Create loading thread
-copy %s to %s
-open %s error !
-/proc/self/maps
-cannot open '%s'
-fstat %s failed: %d
-%s size: %d
-Alloc memory failed
-getJNIEnv by dlsym: %p
-Module %s base: %p
-Function %s offset: 0x%x
-Function %s not found in %s
-(Ljava/lang/String;Ljava/lang/String;Ljava/lang/String;Ljava/lang/ClassLoader;)V
-(Ljava/lang/String;)Ljava/lang/Class;
-Load dex %s to %s, and call %s.%s %s
+ro.build.version.sdk
+[+] Android sdk version: %d
+[+] %p write string: [%d]%s
+ptrace_cont
+[+] X86 ptrace call %p %d
+ptrace_detach
+ptrace_attach
+ptrace_syscall
+[+] Current syscall: %d
+/proc/%d/maps
+Cannot open '%s'
+[+] SDK version: %d
+addr: %d
+/proc/%d/cmdline
+[+] Remote mmap %d bytes
+[+] libc_path: %p
+[+] local_mmap_addr: %p
+[+] Remote mmap addr %p 
+[+] Call mmap result: %p
+[+] Errno addr: %p
+mmap failed: %d
+unhook error: %d
+[+] Injecting process: %d
+__dl___loader_dlopen
+__dl__Z8__dlopenPKciPKv
+__loader_dlopen
+Get dlopen address failed
+dlopen %s error: %d
+Get function %s in %s failed
+Load module %s failed
+readlink 
+[+]libc_path: %s
+[+]linker_path: %s
+[+]libdl_path: %s
+Process %s not found
+Max support 10 params
+p:m:e:P:h
+Target process not specified
+Process %s pid: %d
+[+] Before to inject.
+[+] Before to inject.
+[+] Inject Success.
+[+] Inject Success.
+[+] Inject Failed.
+[+] Inject Failed.
+ptrace_getregs: Can not get register values
+ptrace_setregs: Can not set register values
 symtab_offset=0x%x symtab_entries=0x%x strtab_offset=0x%x
-_ZN7android14AndroidRuntime9getJNIEnvEv
-/system/lib/libandroid_runtime.so
-Must run in Android app process
+[+] Calling mmap in target process %d.
+[+] Inline hook is detected: %p[%d] 
+Alloc memory in target process failed
+[+] Calling dlopen %s in target process.
+[+] Calling dlopen return: %p
+[+] Remote module %s addr: %p
+[+] Remote function %s addr: %p
+[+] Calling function %s in target process.
+[+] Calling target function return: 0x%lx
+[+] Get imports: dlopen: %p, dlclose: %p
+    ./droid_inject -p <target process name or id> -m <target inject module path> -e <module entry funciton> [-P param of module entry funciton]
+Target inject module not specified
+Entry function of module %s not specified
+/system/lib/libdl.so
+/system/bin/linker
+/system/lib/libc.so
 GCC: (GNU) 4.8
 gold 1.11
 .shstrtab
 .rel.dyn
 .rel.plt
+.note.android.ident
 .eh_frame
 .eh_frame_hdr
 .fini_array
 .init_array
+.preinit_array
 .dynamic
 .got.plt
 .comment
 .note.gnu.gold-version
```

#### readelf --wide --decompress --hex-dump=.dynstr {}

```diff
@@ -1,38 +1,30 @@
 
 Hex dump of section '.dynstr':
-  0x00000404 005f5f63 78615f66 696e616c 697a6500 .__cxa_finalize.
-  0x00000414 5f5f6378 615f6174 65786974 005f5f73 __cxa_atexit.__s
-  0x00000424 7461636b 5f63686b 5f666169 6c006c6f tack_chk_fail.lo
-  0x00000434 61645f64 65785f69 6e5f7468 72656164 ad_dex_in_thread
-  0x00000444 005f5f61 6e64726f 69645f6c 6f675f70 .__android_log_p
-  0x00000454 72696e74 00667265 65006c6f 61645f64 rint.free.load_d
-  0x00000464 6578005f 5f737461 636b5f63 686b5f67 ex.__stack_chk_g
-  0x00000474 75617264 00737472 6e637079 00676574 uard.strncpy.get
-  0x00000484 75696400 73707269 6e746600 61636365 uid.sprintf.acce
-  0x00000494 73730067 65745f66 696c655f 73697a65 ss.get_file_size
-  0x000004a4 00676574 5f6a6e69 5f656e76 006d616c .get_jni_env.mal
-  0x000004b4 6c6f6300 70746872 6561645f 63726561 loc.pthread_crea
-  0x000004c4 74650063 686d6f64 00636f70 7966696c te.chmod.copyfil
-  0x000004d4 65006d6b 64697200 4a617661 5f636f6d e.mkdir.Java_com
-  0x000004e4 5f746573 745f616e 64726f69 64737079 _test_androidspy
-  0x000004f4 5f48656c 70657255 74696c5f 6e617469 _HelperUtil_nati
-  0x00000504 76655365 74736964 00736574 73696400 veSetsid.setsid.
-  0x00000514 4a617661 5f636f6d 5f746573 745f616e Java_com_test_an
-  0x00000524 64726f69 64737079 5f48656c 70657255 droidspy_HelperU
-  0x00000534 74696c5f 6e617469 7665556d 61736b00 til_nativeUmask.
-  0x00000544 756d6173 6b007374 61740066 6f70656e umask.stat.fopen
-  0x00000554 00667075 74630067 65746300 66636c6f .fputc.getc.fclo
-  0x00000564 73650067 65745f6d 6f64756c 655f6261 se.get_module_ba
-  0x00000574 73650073 74727374 72006667 65747300 se.strstr.fgets.
-  0x00000584 73747274 6f6b0073 7472746f 756c0067 strtok.strtoul.g
-  0x00000594 65745f73 796d626f 6c5f6f66 66736574 et_symbol_offset
-  0x000005a4 006f7065 6e006673 74617400 6d6d6170 .open.fstat.mmap
-  0x000005b4 006d656d 73657400 72656164 00636c6f .memset.read.clo
-  0x000005c4 73650073 7472636d 70006d75 6e6d6170 se.strcmp.munmap
-  0x000005d4 00646c73 796d005f 65646174 61005f5f .dlsym._edata.__
-  0x000005e4 6273735f 73746172 74005f65 6e64006c bss_start._end.l
-  0x000005f4 69626c6f 672e736f 006c6962 73746463 iblog.so.libstdc
-  0x00000604 2b2b2e73 6f006c69 626d2e73 6f006c69 ++.so.libm.so.li
-  0x00000614 62632e73 6f006c69 62646c2e 736f006c bc.so.libdl.so.l
-  0x00000624 69626465 786c6f61 6465722e 736f00   ibdexloader.so.
+  0x00000438 005f5f6c 6962635f 696e6974 005f5f63 .__libc_init.__c
+  0x00000448 78615f61 74657869 74005f5f 73746163 xa_atexit.__stac
+  0x00000458 6b5f6368 6b5f6661 696c005f 5f737461 k_chk_fail.__sta
+  0x00000468 636b5f63 686b5f67 75617264 005f5f73 ck_chk_guard.__s
+  0x00000478 79737465 6d5f7072 6f706572 74795f67 ystem_property_g
+  0x00000488 65740061 746f6900 7072696e 7466005f et.atoi.printf._
+  0x00000498 5f616e64 726f6964 5f6c6f67 5f707269 _android_log_pri
+  0x000004a8 6e740070 74726163 65006d65 6d637079 nt.ptrace.memcpy
+  0x000004b8 00737472 6c656e00 70657272 6f720077 .strlen.perror.w
+  0x000004c8 61697470 69640073 6e707269 6e746600 aitpid.snprintf.
+  0x000004d8 666f7065 6e007374 72737472 00666765 fopen.strstr.fge
+  0x000004e8 74730066 636c6f73 65007374 72746f6b ts.fclose.strtok
+  0x000004f8 00737472 746f756c 006f7065 6e006673 .strtoul.open.fs
+  0x00000508 74617400 6d616c6c 6f63006d 656d7365 tat.malloc.memse
+  0x00000518 74007265 61640063 6c6f7365 00737472 t.read.close.str
+  0x00000528 636d7000 66726565 005f5f73 46006670 cmp.free.__sF.fp
+  0x00000538 72696e74 6600646c 6f70656e 00646c73 rintf.dlopen.dls
+  0x00000548 796d006f 70656e64 69720072 65616464 ym.opendir.readd
+  0x00000558 69720063 6c6f7365 64697200 73707269 ir.closedir.spri
+  0x00000568 6e746600 66777269 74650072 6561646c ntf.fwrite.readl
+  0x00000578 696e6b00 6c737461 74006765 746f7074 ink.lstat.getopt
+  0x00000588 5f6c6f6e 67006f70 74617267 00667075 _long.optarg.fpu
+  0x00000598 74630070 75747300 5f656461 7461005f tc.puts._edata._
+  0x000005a8 5f627373 5f737461 7274005f 656e6400 _bss_start._end.
+  0x000005b8 6c69626c 6f672e73 6f006c69 62737464 liblog.so.libstd
+  0x000005c8 632b2b2e 736f006c 69626d2e 736f006c c++.so.libm.so.l
+  0x000005d8 6962632e 736f006c 6962646c 2e736f00 ibc.so.libdl.so.
```

#### readelf --wide --decompress --hex-dump=.hash {}

```diff
@@ -1,25 +1,25 @@
 
 Hex dump of section '.hash':
-  0x00000634 25000000 2f000000 00000000 29000000 %.../.......)...
-  0x00000644 00000000 13000000 2a000000 22000000 ........*..."...
-  0x00000654 2b000000 07000000 00000000 00000000 +...............
-  0x00000664 1f000000 24000000 02000000 00000000 ....$...........
-  0x00000674 20000000 1c000000 28000000 21000000  .......(...!...
-  0x00000684 2c000000 0b000000 00000000 27000000 ,...........'...
-  0x00000694 00000000 0f000000 0e000000 00000000 ................
-  0x000006a4 00000000 25000000 0d000000 00000000 ....%...........
-  0x000006b4 1e000000 2e000000 26000000 00000000 ........&.......
-  0x000006c4 00000000 2d000000 04000000 00000000 ....-...........
-  0x000006d4 00000000 00000000 01000000 00000000 ................
-  0x000006e4 00000000 00000000 00000000 00000000 ................
-  0x000006f4 00000000 05000000 00000000 03000000 ................
-  0x00000704 00000000 00000000 00000000 00000000 ................
-  0x00000714 00000000 00000000 00000000 00000000 ................
-  0x00000724 14000000 06000000 0c000000 00000000 ................
-  0x00000734 00000000 00000000 11000000 00000000 ................
-  0x00000744 10000000 17000000 00000000 19000000 ................
-  0x00000754 00000000 00000000 0a000000 08000000 ................
-  0x00000764 12000000 1a000000 23000000 15000000 ........#.......
-  0x00000774 1b000000 00000000 1d000000 18000000 ................
-  0x00000784 09000000 16000000                   ........
+  0x000005e8 25000000 2f000000 00000000 1f000000 %.../...........
+  0x000005f8 26000000 00000000 00000000 00000000 &...............
+  0x00000608 20000000 00000000 00000000 00000000  ...............
+  0x00000618 11000000 16000000 02000000 00000000 ................
+  0x00000628 13000000 25000000 1a000000 14000000 ....%...........
+  0x00000638 2c000000 24000000 00000000 19000000 ,...$...........
+  0x00000648 06000000 17000000 00000000 1d000000 ................
+  0x00000658 00000000 28000000 27000000 0e000000 ....(...'.......
+  0x00000668 10000000 2e000000 2a000000 22000000 ........*..."...
+  0x00000678 00000000 2d000000 29000000 00000000 ....-...).......
+  0x00000688 00000000 00000000 00000000 00000000 ................
+  0x00000698 00000000 01000000 00000000 00000000 ................
+  0x000006a8 00000000 00000000 00000000 07000000 ................
+  0x000006b8 00000000 0b000000 00000000 03000000 ................
+  0x000006c8 00000000 0c000000 0f000000 0d000000 ................
+  0x000006d8 08000000 04000000 00000000 00000000 ................
+  0x000006e8 15000000 00000000 00000000 00000000 ................
+  0x000006f8 05000000 09000000 1b000000 00000000 ................
+  0x00000708 1e000000 21000000 12000000 00000000 ....!...........
+  0x00000718 23000000 0a000000 00000000 00000000 #...............
+  0x00000728 00000000 18000000 00000000 2b000000 ............+...
+  0x00000738 00000000 1c000000                   ........
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.plt {}

```diff
@@ -1,175 +1,210 @@
 
 
 
 Disassembly of section .plt:
 
-000008c0 <__cxa_atexit@plt-0x10>:
+000008f0 <__libc_init@plt-0x10>:
 	push   0x4(%ebx)
 	jmp    *0x8(%ebx)
 	add    %al,(%eax)
 	...
 
-000008d0 <__cxa_atexit@plt>:
+00000900 <__libc_init@plt>:
 	jmp    *0xc(%ebx)
 	push   $0x0
-	jmp    8c0 <__cxa_atexit@plt-0x10>
+	jmp    8f0 <__libc_init@plt-0x10>
 
-000008e0 <__stack_chk_fail@plt>:
+00000910 <__cxa_atexit@plt>:
 	jmp    *0x10(%ebx)
 	push   $0x8
-	jmp    8c0 <__cxa_atexit@plt-0x10>
+	jmp    8f0 <__libc_init@plt-0x10>
 
-000008f0 <__cxa_finalize@plt>:
+00000920 <__stack_chk_fail@plt>:
 	jmp    *0x14(%ebx)
 	push   $0x10
-	jmp    8c0 <__cxa_atexit@plt-0x10>
+	jmp    8f0 <__libc_init@plt-0x10>
 
-00000900 <__android_log_print@plt>:
+00000930 <__system_property_get@plt>:
 	jmp    *0x18(%ebx)
 	push   $0x18
-	jmp    8c0 <__cxa_atexit@plt-0x10>
+	jmp    8f0 <__libc_init@plt-0x10>
 
-00000910 <free@plt>:
+00000940 <atoi@plt>:
 	jmp    *0x1c(%ebx)
 	push   $0x20
-	jmp    8c0 <__cxa_atexit@plt-0x10>
+	jmp    8f0 <__libc_init@plt-0x10>
 
-00000920 <strncpy@plt>:
+00000950 <printf@plt>:
 	jmp    *0x20(%ebx)
 	push   $0x28
-	jmp    8c0 <__cxa_atexit@plt-0x10>
+	jmp    8f0 <__libc_init@plt-0x10>
 
-00000930 <getuid@plt>:
+00000960 <__android_log_print@plt>:
 	jmp    *0x24(%ebx)
 	push   $0x30
-	jmp    8c0 <__cxa_atexit@plt-0x10>
+	jmp    8f0 <__libc_init@plt-0x10>
 
-00000940 <sprintf@plt>:
+00000970 <ptrace@plt>:
 	jmp    *0x28(%ebx)
 	push   $0x38
-	jmp    8c0 <__cxa_atexit@plt-0x10>
+	jmp    8f0 <__libc_init@plt-0x10>
 
-00000950 <access@plt>:
+00000980 <memcpy@plt>:
 	jmp    *0x2c(%ebx)
 	push   $0x40
-	jmp    8c0 <__cxa_atexit@plt-0x10>
+	jmp    8f0 <__libc_init@plt-0x10>
 
-00000960 <malloc@plt>:
+00000990 <strlen@plt>:
 	jmp    *0x30(%ebx)
 	push   $0x48
-	jmp    8c0 <__cxa_atexit@plt-0x10>
+	jmp    8f0 <__libc_init@plt-0x10>
 
-00000970 <pthread_create@plt>:
+000009a0 <perror@plt>:
 	jmp    *0x34(%ebx)
 	push   $0x50
-	jmp    8c0 <__cxa_atexit@plt-0x10>
+	jmp    8f0 <__libc_init@plt-0x10>
 
-00000980 <chmod@plt>:
+000009b0 <waitpid@plt>:
 	jmp    *0x38(%ebx)
 	push   $0x58
-	jmp    8c0 <__cxa_atexit@plt-0x10>
+	jmp    8f0 <__libc_init@plt-0x10>
 
-00000990 <mkdir@plt>:
+000009c0 <snprintf@plt>:
 	jmp    *0x3c(%ebx)
 	push   $0x60
-	jmp    8c0 <__cxa_atexit@plt-0x10>
+	jmp    8f0 <__libc_init@plt-0x10>
 
-000009a0 <setsid@plt>:
+000009d0 <fopen@plt>:
 	jmp    *0x40(%ebx)
 	push   $0x68
-	jmp    8c0 <__cxa_atexit@plt-0x10>
+	jmp    8f0 <__libc_init@plt-0x10>
 
-000009b0 <umask@plt>:
+000009e0 <strstr@plt>:
 	jmp    *0x44(%ebx)
 	push   $0x70
-	jmp    8c0 <__cxa_atexit@plt-0x10>
+	jmp    8f0 <__libc_init@plt-0x10>
 
-000009c0 <stat@plt>:
+000009f0 <fgets@plt>:
 	jmp    *0x48(%ebx)
 	push   $0x78
-	jmp    8c0 <__cxa_atexit@plt-0x10>
+	jmp    8f0 <__libc_init@plt-0x10>
 
-000009d0 <fopen@plt>:
+00000a00 <fclose@plt>:
 	jmp    *0x4c(%ebx)
 	push   $0x80
-	jmp    8c0 <__cxa_atexit@plt-0x10>
+	jmp    8f0 <__libc_init@plt-0x10>
 
-000009e0 <fputc@plt>:
+00000a10 <strtok@plt>:
 	jmp    *0x50(%ebx)
 	push   $0x88
-	jmp    8c0 <__cxa_atexit@plt-0x10>
+	jmp    8f0 <__libc_init@plt-0x10>
 
-000009f0 <getc@plt>:
+00000a20 <strtoul@plt>:
 	jmp    *0x54(%ebx)
 	push   $0x90
-	jmp    8c0 <__cxa_atexit@plt-0x10>
+	jmp    8f0 <__libc_init@plt-0x10>
 
-00000a00 <fclose@plt>:
+00000a30 <open@plt>:
 	jmp    *0x58(%ebx)
 	push   $0x98
-	jmp    8c0 <__cxa_atexit@plt-0x10>
+	jmp    8f0 <__libc_init@plt-0x10>
 
-00000a10 <strstr@plt>:
+00000a40 <fstat@plt>:
 	jmp    *0x5c(%ebx)
 	push   $0xa0
-	jmp    8c0 <__cxa_atexit@plt-0x10>
+	jmp    8f0 <__libc_init@plt-0x10>
 
-00000a20 <fgets@plt>:
+00000a50 <malloc@plt>:
 	jmp    *0x60(%ebx)
 	push   $0xa8
-	jmp    8c0 <__cxa_atexit@plt-0x10>
+	jmp    8f0 <__libc_init@plt-0x10>
 
-00000a30 <strtok@plt>:
+00000a60 <memset@plt>:
 	jmp    *0x64(%ebx)
 	push   $0xb0
-	jmp    8c0 <__cxa_atexit@plt-0x10>
+	jmp    8f0 <__libc_init@plt-0x10>
 
-00000a40 <strtoul@plt>:
+00000a70 <read@plt>:
 	jmp    *0x68(%ebx)
 	push   $0xb8
-	jmp    8c0 <__cxa_atexit@plt-0x10>
+	jmp    8f0 <__libc_init@plt-0x10>
 
-00000a50 <open@plt>:
+00000a80 <close@plt>:
 	jmp    *0x6c(%ebx)
 	push   $0xc0
-	jmp    8c0 <__cxa_atexit@plt-0x10>
+	jmp    8f0 <__libc_init@plt-0x10>
 
-00000a60 <fstat@plt>:
+00000a90 <strcmp@plt>:
 	jmp    *0x70(%ebx)
 	push   $0xc8
-	jmp    8c0 <__cxa_atexit@plt-0x10>
+	jmp    8f0 <__libc_init@plt-0x10>
 
-00000a70 <mmap@plt>:
+00000aa0 <free@plt>:
 	jmp    *0x74(%ebx)
 	push   $0xd0
-	jmp    8c0 <__cxa_atexit@plt-0x10>
+	jmp    8f0 <__libc_init@plt-0x10>
 
-00000a80 <memset@plt>:
+00000ab0 <fprintf@plt>:
 	jmp    *0x78(%ebx)
 	push   $0xd8
-	jmp    8c0 <__cxa_atexit@plt-0x10>
+	jmp    8f0 <__libc_init@plt-0x10>
 
-00000a90 <read@plt>:
+00000ac0 <dlopen@plt>:
 	jmp    *0x7c(%ebx)
 	push   $0xe0
-	jmp    8c0 <__cxa_atexit@plt-0x10>
+	jmp    8f0 <__libc_init@plt-0x10>
 
-00000aa0 <close@plt>:
+00000ad0 <dlsym@plt>:
 	jmp    *0x80(%ebx)
 	push   $0xe8
-	jmp    8c0 <__cxa_atexit@plt-0x10>
+	jmp    8f0 <__libc_init@plt-0x10>
 
-00000ab0 <strcmp@plt>:
+00000ae0 <opendir@plt>:
 	jmp    *0x84(%ebx)
 	push   $0xf0
-	jmp    8c0 <__cxa_atexit@plt-0x10>
+	jmp    8f0 <__libc_init@plt-0x10>
 
-00000ac0 <munmap@plt>:
+00000af0 <readdir@plt>:
 	jmp    *0x88(%ebx)
 	push   $0xf8
-	jmp    8c0 <__cxa_atexit@plt-0x10>
+	jmp    8f0 <__libc_init@plt-0x10>
 
-00000ad0 <dlsym@plt>:
+00000b00 <closedir@plt>:
 	jmp    *0x8c(%ebx)
 	push   $0x100
-	jmp    8c0 <__cxa_atexit@plt-0x10>
+	jmp    8f0 <__libc_init@plt-0x10>
+
+00000b10 <sprintf@plt>:
+	jmp    *0x90(%ebx)
+	push   $0x108
+	jmp    8f0 <__libc_init@plt-0x10>
+
+00000b20 <fwrite@plt>:
+	jmp    *0x94(%ebx)
+	push   $0x110
+	jmp    8f0 <__libc_init@plt-0x10>
+
+00000b30 <readlink@plt>:
+	jmp    *0x98(%ebx)
+	push   $0x118
+	jmp    8f0 <__libc_init@plt-0x10>
+
+00000b40 <lstat@plt>:
+	jmp    *0x9c(%ebx)
+	push   $0x120
+	jmp    8f0 <__libc_init@plt-0x10>
+
+00000b50 <getopt_long@plt>:
+	jmp    *0xa0(%ebx)
+	push   $0x128
+	jmp    8f0 <__libc_init@plt-0x10>
+
+00000b60 <fputc@plt>:
+	jmp    *0xa4(%ebx)
+	push   $0x130
+	jmp    8f0 <__libc_init@plt-0x10>
+
+00000b70 <puts@plt>:
+	jmp    *0xa8(%ebx)
+	push   $0x138
+	jmp    8f0 <__libc_init@plt-0x10>
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text {}

```diff
@@ -1,1042 +1,2200 @@
 
 
 
 Disassembly of section .text:
 
-00000ae0 <load_dex_in_thread-0xc0>:
+00000b80 <.text>:
+	push   %ebp
+	mov    $0x18,%ecx
+	mov    %esp,%ebp
+	push   %edi
+	push   %esi
 	push   %ebx
-	call   b90 <dlsym@plt+0xc0>
-	add    $0x348a,%ebx
-	lea    -0x18(%esp),%esp
-	lea    0x90(%ebx),%eax
+	call   114b <puts@plt+0x5db>
+	add    $0x43c4,%ebx
+	and    $0xfffffff0,%esp
+	lea    0xac(%ebx),%esi
+	lea    -0xd0(%esp),%esp
+	lea    0x32c(%ebx),%edx
+	mov    %edx,0x38(%esp)
+	lea    0x70(%esp),%edi
+	mov    %edi,0x3c(%esp)
+	rep movsl %ds:(%esi),%es:(%edi)
+	mov    %edx,(%esp)
+	lea    0x22c(%ebx),%edi
+	mov    %ecx,0x34(%esp)
+	lea    0x12c(%ebx),%esi
+	call   2cd0 <puts@plt+0x2160>
+	mov    %edi,(%esp)
+	call   2cd0 <puts@plt+0x2160>
+	mov    %esi,(%esp)
+	call   2cd0 <puts@plt+0x2160>
+	mov    0x38(%esp),%edx
+	lea    -0x1f65(%ebx),%ecx
+	mov    %ecx,(%esp)
+	mov    %ecx,0x38(%esp)
+	mov    %edx,0x4(%esp)
+	mov    %edx,0x30(%esp)
+	call   950 <printf@plt>
+	mov    0x30(%esp),%edx
+	mov    0x38(%esp),%ecx
+	movl   $0x3,(%esp)
+	mov    %edx,0xc(%esp)
+	lea    -0x21da(%ebx),%edx
+	mov    %ecx,0x8(%esp)
+	mov    %edx,0x4(%esp)
+	mov    %edx,0x38(%esp)
+	call   960 <__android_log_print@plt>
+	mov    %edi,0x4(%esp)
+	lea    -0x1f53(%ebx),%edx
+	mov    %edx,(%esp)
+	mov    %edx,0x30(%esp)
+	call   950 <printf@plt>
+	mov    0x30(%esp),%edx
+	mov    %edi,0xc(%esp)
+	lea    -0x1f3f(%ebx),%edi
+	movl   $0x3,(%esp)
+	mov    %edx,0x8(%esp)
+	mov    0x38(%esp),%edx
+	mov    %edx,0x4(%esp)
+	call   960 <__android_log_print@plt>
+	mov    %esi,0x4(%esp)
+	mov    %edi,(%esp)
+	call   950 <printf@plt>
+	mov    0x38(%esp),%edx
+	mov    %esi,0xc(%esp)
+	lea    -0x1f00(%ebx),%esi
+	mov    %edi,0x8(%esp)
+	lea    0x48(%esp),%edi
+	movl   $0x3,(%esp)
+	mov    %edx,0x4(%esp)
+	call   960 <__android_log_print@plt>
+	mov    0x34(%esp),%eax
+	mov    $0xa,%ecx
+	mov    %edi,0x24(%esp)
+	movl   $0x0,0x2c(%esp)
+	movl   $0x0,0x34(%esp)
+	movl   $0x0,0x30(%esp)
+	movl   $0x0,0x28(%esp)
+	rep stos %eax,%es:(%edi)
+	mov    $0xffffffff,%edi
+	mov    0x3c(%esp),%eax
+	movl   $0x0,0x10(%esp)
+	mov    %esi,0x8(%esp)
+	mov    %eax,0xc(%esp)
+	mov    0xc(%ebp),%eax
+	mov    %eax,0x4(%esp)
+	mov    0x8(%ebp),%eax
 	mov    %eax,(%esp)
-	call   8f0 <__cxa_finalize@plt>
-	lea    0x18(%esp),%esp
+	call   b50 <getopt_long@plt>
+	cmp    $0xffffffff,%eax
+	je     e21 <puts@plt+0x2b1>
+	sub    $0x50,%eax
+	cmp    $0x20,%eax
+	ja     dd6 <puts@plt+0x266>
+	mov    -0x1b18(%ebx,%eax,4),%eax
+	add    %ebx,%eax
+	jmp    *%eax
+	mov    -0x4(%ebx),%eax
+	or     $0xffffffff,%ecx
+	mov    (%eax),%edx
+	xor    %eax,%eax
+	mov    %edx,%edi
+	repnz scas %es:(%edi),%al
+	mov    %ecx,%eax
+	not    %eax
+	mov    %eax,%edi
+	xor    %eax,%eax
+	sub    $0x1,%edi
+	jmp    d43 <puts@plt+0x1d3>
+	movzbl (%edx,%eax,1),%ecx
+	sub    $0x30,%ecx
+	cmp    $0x9,%cl
+	ja     df6 <puts@plt+0x286>
+	add    $0x1,%eax
+	cmp    %edi,%eax
+	jne    d30 <puts@plt+0x1c0>
+	mov    %edx,(%esp)
+	call   940 <atoi@plt>
+	mov    %eax,%edi
+	jmp    ccc <puts@plt+0x15c>
+	mov    -0x4(%ebx),%eax
+	mov    (%eax),%eax
+	mov    %eax,0x30(%esp)
+	jmp    ccc <puts@plt+0x15c>
+	mov    -0xc(%ebx),%eax
+	movl   $0x98,0x8(%esp)
+	movl   $0x1,0x4(%esp)
+	add    $0xa8,%eax
+	mov    %eax,0xc(%esp)
+	lea    -0x1c04(%ebx),%eax
+	mov    %eax,(%esp)
+	call   b20 <fwrite@plt>
+	xor    %eax,%eax
+	lea    -0xc(%ebp),%esp
 	pop    %ebx
+	pop    %esi
+	pop    %edi
+	pop    %ebp
 	ret
+	mov    -0x4(%ebx),%eax
+	mov    (%eax),%eax
+	mov    %eax,0x2c(%esp)
+	jmp    ccc <puts@plt+0x15c>
+	cmpl   $0x9,0x34(%esp)
+	jg     f49 <puts@plt+0x3d9>
+	mov    -0x4(%ebx),%eax
+	mov    0x34(%esp),%edx
+	mov    (%eax),%eax
+	mov    %eax,0x48(%esp,%edx,4)
+	lea    0x1(%edx),%eax
+	mov    %eax,0x34(%esp)
+	jmp    ccc <puts@plt+0x15c>
+	mov    -0xc(%ebx),%eax
+	movl   $0xa,(%esp)
+	add    $0xa8,%eax
+	mov    %eax,0x4(%esp)
+	call   b60 <fputc@plt>
+	or     $0xffffffff,%eax
+	jmp    d96 <puts@plt+0x226>
+	cmp    %eax,%edi
+	jbe    d47 <puts@plt+0x1d7>
+	mov    %edx,(%esp)
+	mov    %edx,0x28(%esp)
+	call   1f50 <puts@plt+0x13e0>
+	test   %eax,%eax
+	mov    %eax,%edi
+	mov    0x28(%esp),%edx
+	js     f7e <puts@plt+0x40e>
+	mov    %edx,0x28(%esp)
+	jmp    ccc <puts@plt+0x15c>
+	test   %edi,%edi
+	js     faf <puts@plt+0x43f>
+	mov    0x28(%esp),%eax
+	test   %eax,%eax
+	je     e6b <puts@plt+0x2fb>
+	mov    %edi,0x8(%esp)
+	lea    -0x1ed8(%ebx),%esi
+	mov    %eax,0x4(%esp)
+	mov    %esi,(%esp)
+	call   950 <printf@plt>
+	mov    0x28(%esp),%eax
+	mov    %edi,0x10(%esp)
+	mov    %esi,0x8(%esp)
+	mov    %eax,0xc(%esp)
+	mov    0x38(%esp),%eax
+	movl   $0x3,(%esp)
+	mov    %eax,0x4(%esp)
+	call   960 <__android_log_print@plt>
+	cmpl   $0x0,0x30(%esp)
+	je     1034 <puts@plt+0x4c4>
+	cmpl   $0x0,0x2c(%esp)
+	je     fe4 <puts@plt+0x474>
+	lea    -0x1ec4(%ebx),%eax
+	mov    %eax,(%esp)
+	call   b70 <puts@plt>
+	movl   $0x3,(%esp)
+	lea    -0x1eae(%ebx),%eax
+	mov    %eax,0x8(%esp)
+	mov    0x38(%esp),%eax
+	mov    %eax,0x4(%esp)
+	call   960 <__android_log_print@plt>
+	mov    0x34(%esp),%eax
+	movl   $0x1,0x14(%esp)
+	mov    %edi,(%esp)
+	mov    %eax,0x10(%esp)
+	mov    0x24(%esp),%eax
+	mov    %eax,0xc(%esp)
+	mov    0x2c(%esp),%eax
+	mov    %eax,0x8(%esp)
+	mov    0x30(%esp),%eax
+	mov    %eax,0x4(%esp)
+	call   2580 <puts@plt+0x1a10>
+	test   %eax,%eax
+	mov    %eax,%esi
+	jne    f16 <puts@plt+0x3a6>
+	lea    -0x1e97(%ebx),%eax
+	mov    %eax,(%esp)
+	call   b70 <puts@plt>
+	movl   $0x3,(%esp)
+	lea    -0x1e83(%ebx),%eax
+	mov    %eax,0x8(%esp)
+	mov    0x38(%esp),%eax
+	mov    %eax,0x4(%esp)
+	call   960 <__android_log_print@plt>
+	xor    %eax,%eax
+	jmp    d96 <puts@plt+0x226>
+	lea    -0x1e6e(%ebx),%eax
+	mov    %eax,(%esp)
+	call   b70 <puts@plt>
+	movl   $0x3,(%esp)
+	lea    -0x1e5b(%ebx),%eax
+	mov    %eax,0x8(%esp)
+	mov    0x38(%esp),%eax
+	mov    %eax,0x4(%esp)
+	call   960 <__android_log_print@plt>
+	mov    %esi,%eax
+	jmp    d96 <puts@plt+0x226>
+	mov    -0xc(%ebx),%eax
+	movl   $0x15,0x8(%esp)
+	movl   $0x1,0x4(%esp)
+	add    $0xa8,%eax
+	mov    %eax,0xc(%esp)
+	lea    -0x1f16(%ebx),%eax
+	mov    %eax,(%esp)
+	call   b20 <fwrite@plt>
+	or     $0xffffffff,%eax
+	jmp    d96 <puts@plt+0x226>
+	mov    -0x4(%ebx),%eax
+	mov    (%eax),%eax
+	mov    %eax,0x8(%esp)
+	lea    -0x1f2c(%ebx),%eax
+	mov    %eax,0x4(%esp)
+	mov    -0xc(%ebx),%eax
+	add    $0xa8,%eax
+	mov    %eax,(%esp)
+	call   ab0 <fprintf@plt>
+	or     $0xffffffff,%eax
+	jmp    d96 <puts@plt+0x226>
+	mov    -0xc(%ebx),%eax
+	movl   $0x1d,0x8(%esp)
+	movl   $0x1,0x4(%esp)
+	add    $0xa8,%eax
+	mov    %eax,0xc(%esp)
+	lea    -0x1ef6(%ebx),%eax
+	mov    %eax,(%esp)
+	call   b20 <fwrite@plt>
+	or     $0xffffffff,%eax
+	jmp    d96 <puts@plt+0x226>
+	mov    0x30(%esp),%eax
+	mov    %eax,0x8(%esp)
+	lea    -0x1b44(%ebx),%eax
+	mov    %eax,0x4(%esp)
+	mov    -0xc(%ebx),%eax
+	lea    0xa8(%eax),%esi
+	mov    %esi,(%esp)
+	call   ab0 <fprintf@plt>
+	mov    %esi,0xc(%esp)
+	lea    -0x1c04(%ebx),%eax
+	movl   $0x98,0x8(%esp)
+	movl   $0x1,0x4(%esp)
+	mov    %eax,(%esp)
+	call   b20 <fwrite@plt>
+	or     $0xffffffff,%eax
+	jmp    d96 <puts@plt+0x226>
+	mov    -0xc(%ebx),%eax
+	movl   $0x23,0x8(%esp)
+	movl   $0x1,0x4(%esp)
+	lea    0xa8(%eax),%esi
+	lea    -0x1b68(%ebx),%eax
+	mov    %esi,0xc(%esp)
+	mov    %eax,(%esp)
+	call   b20 <fwrite@plt>
+	jmp    100a <puts@plt+0x49a>
 	...
 	lea    -0xc(%esp),%esp
 	mov    0x10(%esp),%eax
 	test   %eax,%eax
-	je     b1e <dlsym@plt+0x4e>
+	je     107e <puts@plt+0x50e>
 	call   *%eax
 	lea    0xc(%esp),%esp
 	ret
 	lea    0x0(%esi),%esi
 	lea    0x0(%edi,%eiz,1),%edi
+	push   %ebp
+	mov    %esp,%ebp
 	push   %ebx
-	call   b90 <dlsym@plt+0xc0>
-	add    $0x343a,%ebx
+	call   114b <puts@plt+0x5db>
+	add    $0x3ebb,%ebx
+	and    $0xfffffff0,%esp
+	lea    -0x20(%esp),%esp
+	mov    -0x20(%ebx),%eax
+	movl   $0x0,0x4(%esp)
+	mov    %eax,0x14(%esp)
+	mov    -0x1c(%ebx),%eax
+	mov    %eax,0x18(%esp)
+	mov    -0x18(%ebx),%eax
+	mov    %eax,0x1c(%esp)
+	lea    0x14(%esp),%eax
+	mov    %eax,0xc(%esp)
+	mov    -0x14(%ebx),%eax
+	mov    %eax,0x8(%esp)
+	lea    0x4(%ebp),%eax
+	mov    %eax,(%esp)
+	call   900 <__libc_init@plt>
+	lea    0x0(%esi,%eiz,1),%esi
+	push   %ebx
+	call   114b <puts@plt+0x5db>
+	add    $0x3e5e,%ebx
 	lea    -0x18(%esp),%esp
-	lea    0x90(%ebx),%eax
+	lea    0x42c(%ebx),%eax
 	mov    %eax,0x8(%esp)
 	mov    0x20(%esp),%eax
 	mov    %eax,0x4(%esp)
-	lea    -0x3460(%ebx),%eax
+	lea    -0x3ee4(%ebx),%eax
 	mov    %eax,(%esp)
-	call   8d0 <__cxa_atexit@plt>
+	call   910 <__cxa_atexit@plt>
 	lea    0x18(%esp),%esp
 	pop    %ebx
 	ret
 	lea    0x0(%esi),%esi
 	lea    0x0(%edi,%eiz,1),%edi
 	push   %ebx
-	call   b90 <dlsym@plt+0xc0>
-	add    $0x33fa,%ebx
+	call   114b <puts@plt+0x5db>
+	add    $0x3e1e,%ebx
 	lea    -0x8(%esp),%esp
-	call   8e0 <__stack_chk_fail@plt>
+	call   920 <__stack_chk_fail@plt>
 	lea    0x8(%esp),%esp
 	pop    %ebx
 	ret
-	nop
-	lea    0x0(%esi,%eiz,1),%esi
 	mov    (%esp),%ebx
 	ret
 	nop
-	lea    0x0(%esi,%eiz,1),%esi
-	add    %al,(%eax)
-	...
-
-00000ba0 <load_dex_in_thread>:
-	push   %ebp
 	push   %edi
 	push   %esi
 	push   %ebx
-	call   b90 <dlsym@plt+0xc0>
-	add    $0x33c7,%ebx
-	lea    -0x4c(%esp),%esp
-	lea    -0x251c(%ebx),%eax
-	mov    %eax,0x8(%esp)
-	lea    -0x250f(%ebx),%ebp
-	movl   $0x4,(%esp)
-	mov    %ebp,0x4(%esp)
-	call   900 <__android_log_print@plt>
-	mov    0x60(%esp),%eax
-	lea    0x3c(%esp),%edx
-	movl   $0x0,0x3c(%esp)
-	mov    (%eax),%eax
-	mov    %eax,0x2c(%esp)
-	mov    %eax,%edi
-	mov    (%eax),%eax
-	movl   $0x0,0x8(%esp)
-	mov    %edx,0x4(%esp)
-	mov    %edi,(%esp)
-	call   *0x10(%eax)
-	mov    0x3c(%esp),%eax
+	call   114b <puts@plt+0x5db>
+	add    $0x3dfc,%ebx
+	lea    -0x20(%esp),%esp
+	mov    -0x10(%ebx),%esi
+	mov    (%esi),%eax
+	mov    %eax,0x1c(%esp)
+	mov    0x430(%ebx),%eax
 	test   %eax,%eax
-	je     ed0 <load_dex_in_thread+0x330>
-	mov    %eax,0xc(%esp)
-	lea    -0x24f6(%ebx),%eax
-	mov    %ebp,0x4(%esp)
-	movl   $0x4,(%esp)
-	mov    %eax,0x8(%esp)
-	call   900 <__android_log_print@plt>
-	mov    0x3c(%esp),%eax
-	lea    -0x24e3(%ebx),%ecx
-	mov    (%eax),%edx
-	mov    %ecx,0x4(%esp)
-	mov    %eax,(%esp)
-	call   *0x18(%edx)
-	lea    -0x24cd(%ebx),%ecx
-	mov    %eax,%esi
-	mov    0x3c(%esp),%eax
-	mov    (%eax),%edx
-	mov    %ecx,0xc(%esp)
-	lea    -0x24b3(%ebx),%ecx
-	mov    %esi,0x4(%esp)
-	mov    %eax,(%esp)
-	mov    %ecx,0x8(%esp)
-	call   *0x1c4(%edx)
-	mov    0x3c(%esp),%edx
-	mov    (%edx),%ecx
-	mov    %esi,0x4(%esp)
-	mov    %edx,(%esp)
-	mov    %eax,0x8(%esp)
-	call   *0x1c8(%ecx)
-	mov    0x60(%esp),%esi
-	mov    %eax,0x24(%esp)
-	mov    0x3c(%esp),%eax
-	lea    0x4(%esi),%ecx
-	mov    (%eax),%edx
-	mov    %ecx,0x4(%esp)
-	mov    %eax,(%esp)
-	call   *0x29c(%edx)
-	mov    0x60(%esp),%edi
-	mov    %eax,0x28(%esp)
-	mov    0x3c(%esp),%eax
-	lea    0x108(%edi),%ecx
-	mov    (%eax),%edx
-	mov    %ecx,0x4(%esp)
-	mov    %eax,(%esp)
-	call   *0x29c(%edx)
-	lea    -0x249e(%ebx),%ecx
-	mov    %eax,%edi
-	mov    0x3c(%esp),%eax
-	mov    (%eax),%edx
-	mov    %ecx,0x4(%esp)
-	mov    %eax,(%esp)
-	call   *0x18(%edx)
-	mov    0x3c(%esp),%edx
-	lea    -0x22f0(%ebx),%ecx
-	mov    %eax,%esi
-	mov    (%edx),%eax
-	mov    %ecx,0xc(%esp)
-	lea    -0x2481(%ebx),%ecx
-	mov    %esi,0x4(%esp)
-	mov    %edx,(%esp)
-	mov    %ecx,0x8(%esp)
-	call   *0x84(%eax)
-	mov    0x3c(%esp),%ecx
-	mov    0x24(%esp),%edx
-	mov    (%ecx),%ecx
-	mov    %edi,0x10(%esp)
-	mov    %eax,0x8(%esp)
-	mov    0x28(%esp),%edi
-	mov    0x3c(%esp),%eax
-	mov    %edx,0x18(%esp)
-	mov    %esi,0x4(%esp)
-	movl   $0x0,0x14(%esp)
-	mov    %edi,0xc(%esp)
-	mov    %eax,(%esp)
-	call   *0x70(%ecx)
-	mov    %ebp,0x4(%esp)
-	movl   $0x4,(%esp)
-	mov    %eax,0xc(%esp)
-	mov    %eax,%edi
-	lea    -0x247a(%ebx),%eax
-	mov    %eax,0x8(%esp)
-	call   900 <__android_log_print@plt>
-	mov    0x3c(%esp),%eax
-	lea    -0x229c(%ebx),%ecx
-	mov    (%eax),%edx
-	mov    %ecx,0xc(%esp)
-	lea    -0x2464(%ebx),%ecx
-	mov    %esi,0x4(%esp)
-	mov    %eax,(%esp)
-	mov    %ecx,0x8(%esp)
-	call   *0x84(%edx)
-	mov    0x60(%esp),%esi
-	mov    %eax,0x24(%esp)
-	mov    0x3c(%esp),%eax
-	add    $0x20c,%esi
-	mov    (%eax),%edx
-	mov    %esi,0x4(%esp)
-	mov    %eax,(%esp)
-	call   *0x29c(%edx)
-	mov    0x3c(%esp),%edx
-	mov    (%edx),%ecx
-	mov    %eax,0xc(%esp)
-	mov    0x24(%esp),%eax
-	mov    %edx,(%esp)
+	jne    11ef <puts@plt+0x67f>
+	lea    0x12(%esp),%edi
+	lea    -0x220c(%ebx),%eax
 	mov    %edi,0x4(%esp)
-	mov    %eax,0x8(%esp)
-	call   *0x88(%ecx)
-	mov    %esi,0xc(%esp)
-	mov    %ebp,0x4(%esp)
-	mov    %eax,0x10(%esp)
-	mov    %eax,%edi
-	movl   $0x4,(%esp)
-	lea    -0x245a(%ebx),%eax
-	mov    %eax,0x8(%esp)
-	call   900 <__android_log_print@plt>
-	mov    0x3c(%esp),%eax
-	mov    (%eax),%edx
 	mov    %eax,(%esp)
-	call   *0x3c(%edx)
+	movl   $0x0,0x12(%esp)
+	movl   $0x0,0x16(%esp)
+	movw   $0x0,0x1a(%esp)
+	call   930 <__system_property_get@plt>
+	mov    %edi,(%esp)
+	lea    -0x21f7(%ebx),%edi
+	call   940 <atoi@plt>
+	mov    %eax,0x4(%esp)
+	mov    %edi,(%esp)
+	mov    %eax,0x430(%ebx)
+	call   950 <printf@plt>
+	mov    0x430(%ebx),%eax
+	mov    %edi,0x8(%esp)
+	movl   $0x3,(%esp)
+	mov    %eax,0xc(%esp)
+	lea    -0x21da(%ebx),%eax
+	mov    %eax,0x4(%esp)
+	call   960 <__android_log_print@plt>
+	mov    0x430(%ebx),%eax
+	mov    0x1c(%esp),%ecx
+	mov    (%esi),%edx
+	cmp    %edx,%ecx
+	jne    1201 <puts@plt+0x691>
+	lea    0x20(%esp),%esp
+	pop    %ebx
+	pop    %esi
+	pop    %edi
+	ret
+	call   1130 <puts@plt+0x5c0>
+	lea    0x0(%esi),%esi
+	lea    0x0(%edi,%eiz,1),%edi
+	push   %ebp
+	push   %edi
+	push   %esi
+	push   %ebx
+	call   114b <puts@plt+0x5db>
+	add    $0x3d3b,%ebx
+	lea    -0x3c(%esp),%esp
+	mov    0x5c(%esp),%ebp
+	mov    %ebp,%eax
+	and    $0x3,%eax
+	shr    $0x2,%ebp
+	mov    %eax,0x1c(%esp)
+	mov    %ebp,0x18(%esp)
+	je     1291 <puts@plt+0x721>
+	mov    0x58(%esp),%edi
+	xor    %esi,%esi
+	mov    0x54(%esp),%ebp
+	lea    0x0(%esi),%esi
+	lea    0x0(%edi,%eiz,1),%edi
+	mov    0x50(%esp),%eax
+	add    $0x1,%esi
+	mov    %ebp,0x8(%esp)
+	add    $0x4,%edi
+	movl   $0x0,0xc(%esp)
+	add    $0x4,%ebp
+	movl   $0x1,(%esp)
+	mov    %eax,0x4(%esp)
+	call   970 <ptrace@plt>
+	mov    %eax,-0x4(%edi)
+	cmp    0x18(%esp),%esi
+	mov    %eax,0x2c(%esp)
+	jne    1250 <puts@plt+0x6e0>
+	shl    $0x2,%esi
+	add    %esi,0x54(%esp)
+	add    %esi,0x58(%esp)
+	mov    0x1c(%esp),%eax
 	test   %eax,%eax
-	mov    0x3c(%esp),%eax
-	mov    (%eax),%edx
-	je     e30 <load_dex_in_thread+0x290>
-	mov    %eax,(%esp)
-	call   *0x40(%edx)
-	mov    0x3c(%esp),%eax
-	mov    (%eax),%edx
-	mov    %eax,(%esp)
-	call   *0x44(%edx)
-	mov    %esi,0xc(%esp)
-	lea    -0x244d(%ebx),%eax
-	mov    %ebp,0x4(%esp)
-	movl   $0x6,(%esp)
+	je     12dd <puts@plt+0x76d>
+	mov    0x54(%esp),%eax
+	movl   $0x0,0xc(%esp)
+	movl   $0x1,(%esp)
 	mov    %eax,0x8(%esp)
-	call   900 <__android_log_print@plt>
-	lea    0x4c(%esp),%esp
+	mov    0x50(%esp),%eax
+	mov    %eax,0x4(%esp)
+	call   970 <ptrace@plt>
+	mov    %eax,0x2c(%esp)
+	lea    0x2c(%esp),%eax
+	mov    0x1c(%esp),%edx
+	mov    %eax,0x4(%esp)
+	mov    0x58(%esp),%eax
+	mov    %edx,0x8(%esp)
+	mov    %eax,(%esp)
+	call   980 <memcpy@plt>
+	lea    0x3c(%esp),%esp
 	xor    %eax,%eax
 	pop    %ebx
 	pop    %esi
 	pop    %edi
 	pop    %ebp
 	ret
 	nop
-	mov    0x60(%esp),%esi
-	mov    %edi,0x4(%esp)
-	mov    %eax,(%esp)
-	lea    0x414(%esi),%ecx
-	mov    %ecx,0xc(%esp)
-	lea    0x310(%esi),%ecx
-	mov    %ecx,0x8(%esp)
-	call   *0x1c4(%edx)
-	mov    0x60(%esp),%ecx
-	mov    %eax,%esi
-	mov    0x3c(%esp),%eax
-	add    $0x518,%ecx
-	mov    (%eax),%edx
-	mov    %ecx,0x4(%esp)
-	mov    %eax,(%esp)
-	call   *0x29c(%edx)
-	mov    0x3c(%esp),%edx
-	mov    (%edx),%ecx
-	mov    %edx,(%esp)
-	mov    %eax,0xc(%esp)
-	mov    %esi,0x8(%esp)
-	mov    %edi,0x4(%esp)
-	call   *0x234(%ecx)
-	mov    0x2c(%esp),%esi
-	mov    (%esi),%eax
-	mov    %esi,(%esp)
-	call   *0x14(%eax)
-	mov    0x60(%esp),%eax
-	mov    %eax,(%esp)
-	call   910 <free@plt>
-	mov    %ebp,0x4(%esp)
-	lea    -0x2438(%ebx),%eax
+	lea    0x0(%esi,%eiz,1),%esi
+	push   %ebp
+	push   %edi
+	push   %esi
+	push   %ebx
+	call   114b <puts@plt+0x5db>
+	add    $0x3c5b,%ebx
+	lea    -0x3c(%esp),%esp
+	mov    0x5c(%esp),%eax
+	mov    %eax,%edx
+	and    $0x3,%edx
+	shr    $0x2,%eax
+	mov    %edx,0x1c(%esp)
+	mov    %eax,0x14(%esp)
+	je     1383 <puts@plt+0x813>
+	mov    0x58(%esp),%edi
+	lea    0x2c(%esp),%eax
+	mov    0x54(%esp),%ebp
+	xor    %esi,%esi
+	mov    %eax,0x18(%esp)
+	mov    %edi,%eax
+	mov    %ebp,%edi
+	mov    %eax,%ebp
+	jmp    1340 <puts@plt+0x7d0>
+	nop
+	nop
+	nop
+	nop
+	nop
+	nop
+	nop
+	nop
+	nop
+	nop
+	nop
+	nop
+	nop
+	mov    0x0(%ebp),%eax
+	add    $0x1,%esi
+	mov    0x18(%esp),%ecx
+	add    $0x4,%ebp
+	mov    %eax,(%ecx)
+	mov    0x2c(%esp),%eax
+	mov    %edi,0x8(%esp)
+	add    $0x4,%edi
 	movl   $0x4,(%esp)
-	mov    %eax,0x8(%esp)
-	call   900 <__android_log_print@plt>
-	lea    0x4c(%esp),%esp
+	mov    %eax,0xc(%esp)
+	mov    0x50(%esp),%eax
+	mov    %eax,0x4(%esp)
+	call   970 <ptrace@plt>
+	cmp    0x14(%esp),%esi
+	jne    1340 <puts@plt+0x7d0>
+	shl    $0x2,%esi
+	add    %esi,0x54(%esp)
+	add    %esi,0x58(%esp)
+	mov    0x1c(%esp),%eax
+	test   %eax,%eax
+	jne    1398 <puts@plt+0x828>
+	lea    0x3c(%esp),%esp
 	xor    %eax,%eax
 	pop    %ebx
 	pop    %esi
 	pop    %edi
 	pop    %ebp
 	ret
-	lea    0x0(%esi,%eiz,1),%esi
-	mov    %ebp,0x4(%esp)
-	lea    -0x2505(%ebx),%eax
-	movl   $0x6,(%esp)
+	xchg   %ax,%ax
+	mov    0x54(%esp),%eax
+	movl   $0x0,0xc(%esp)
+	movl   $0x1,(%esp)
+	mov    %eax,0x8(%esp)
+	mov    0x50(%esp),%eax
+	mov    %eax,0x4(%esp)
+	call   970 <ptrace@plt>
+	mov    %eax,0x2c(%esp)
+	lea    0x2c(%esp),%edx
+	mov    0x1c(%esp),%ecx
+	xor    %eax,%eax
+	mov    0x58(%esp),%esi
+	mov    %edx,%edi
+	movzbl (%esi,%eax,1),%edx
+	mov    %dl,(%edi,%eax,1)
+	add    $0x1,%eax
+	cmp    %ecx,%eax
+	jne    13d0 <puts@plt+0x860>
+	mov    0x2c(%esp),%eax
+	movl   $0x4,(%esp)
+	mov    %eax,0xc(%esp)
+	mov    0x54(%esp),%eax
 	mov    %eax,0x8(%esp)
-	call   900 <__android_log_print@plt>
-	lea    0x4c(%esp),%esp
+	mov    0x50(%esp),%eax
+	mov    %eax,0x4(%esp)
+	call   970 <ptrace@plt>
+	lea    0x3c(%esp),%esp
 	xor    %eax,%eax
 	pop    %ebx
 	pop    %esi
 	pop    %edi
 	pop    %ebp
 	ret
-	lea    0x0(%esi,%eiz,1),%esi
-	lea    0x0(%edi,%eiz,1),%edi
-
-00000f00 <load_dex>:
+	lea    0x0(%esi),%esi
 	push   %ebp
 	push   %edi
 	push   %esi
 	push   %ebx
-	call   b90 <dlsym@plt+0xc0>
-	add    $0x3067,%ebx
-	lea    -0x36c(%esp),%esp
-	mov    0x380(%esp),%eax
-	mov    %eax,0x2c(%esp)
-	mov    %eax,%ecx
-	mov    0x384(%esp),%eax
-	mov    %eax,0x24(%esp)
-	mov    %eax,%esi
-	mov    0x388(%esp),%eax
-	mov    %eax,0x30(%esp)
-	mov    %eax,%edx
-	mov    0x38c(%esp),%eax
-	mov    %eax,0x34(%esp)
-	mov    %eax,%edi
-	mov    0x390(%esp),%eax
-	mov    %eax,0x38(%esp)
-	mov    0x394(%esp),%eax
-	mov    %eax,0x3c(%esp)
-	mov    %eax,%ebp
-	mov    -0x8(%ebx),%eax
-	mov    (%eax),%eax
-	mov    %ebp,0x1c(%esp)
-	lea    -0x250f(%ebx),%ebp
-	mov    %edi,0x18(%esp)
-	lea    0x50(%esp),%edi
-	mov    %eax,0x35c(%esp)
-	lea    -0x2274(%ebx),%eax
-	mov    %edx,0x14(%esp)
-	mov    %esi,0x10(%esp)
-	mov    %ecx,0xc(%esp)
-	mov    %ebp,0x4(%esp)
-	movl   $0x4,(%esp)
-	mov    %eax,0x8(%esp)
-	call   900 <__android_log_print@plt>
-	xor    %eax,%eax
-	mov    $0x41,%ecx
-	rep stos %eax,%es:(%edi)
-	mov    %esi,0x4(%esp)
-	lea    0x50(%esp),%esi
-	movl   $0x104,0x8(%esp)
+	call   114b <puts@plt+0x5db>
+	add    $0x3b3b,%ebx
+	lea    -0x2c(%esp),%esp
+	lea    -0x21d3(%ebx),%ebp
+	mov    0x48(%esp),%esi
+	mov    0x44(%esp),%edi
 	mov    %esi,(%esp)
-	call   920 <strncpy@plt>
-	mov    %esi,%eax
-	lea    0x0(%esi,%eiz,1),%esi
-	cmpb   $0x0,(%eax)
-	je     fe8 <load_dex+0xe8>
-	add    $0x1,%eax
-	jne    fd0 <load_dex+0xd0>
-	mov    $0xffffffff,%eax
-	nop
-	cmpb   $0x2f,(%eax)
-	lea    0x1(%eax),%edx
-	je     ff2 <load_dex+0xf2>
-	sub    $0x1,%eax
-	jne    fe0 <load_dex+0xe0>
-	mov    $0x1,%edx
-	movb   $0x0,(%eax)
-	lea    0x154(%esp),%edi
-	mov    $0x41,%ecx
-	xor    %eax,%eax
-	rep stos %eax,%es:(%edi)
-	mov    %edx,0x4(%esp)
-	lea    0x154(%esp),%edx
-	movl   $0x104,0x8(%esp)
-	mov    %edx,(%esp)
-	mov    %edx,0x28(%esp)
-	call   920 <strncpy@plt>
-	call   930 <getuid@plt>
-	mov    %eax,0xc(%esp)
-	lea    -0x242c(%ebx),%eax
-	mov    %esi,0x8(%esp)
+	call   990 <strlen@plt>
+	mov    %eax,0x8(%esp)
+	mov    %esi,0xc(%esp)
+	mov    %edi,0x4(%esp)
+	mov    %ebp,(%esp)
+	call   950 <printf@plt>
 	mov    %esi,(%esp)
+	call   990 <strlen@plt>
+	mov    %eax,0x10(%esp)
+	lea    -0x21da(%ebx),%eax
+	mov    %esi,0x14(%esp)
+	mov    %edi,0xc(%esp)
+	mov    %ebp,0x8(%esp)
+	movl   $0x3,(%esp)
 	mov    %eax,0x4(%esp)
-	call   940 <sprintf@plt>
-	mov    %esi,0xc(%esp)
-	lea    -0x2426(%ebx),%eax
-	mov    %ebp,0x4(%esp)
-	movl   $0x4,(%esp)
-	mov    %eax,0x8(%esp)
-	call   900 <__android_log_print@plt>
-	movl   $0x0,0x4(%esp)
+	call   960 <__android_log_print@plt>
 	mov    %esi,(%esp)
-	call   950 <access@plt>
-	mov    0x28(%esp),%edx
-	cmp    $0xffffffff,%eax
-	je     1298 <load_dex+0x398>
-	xor    %eax,%eax
-	lea    0x258(%esp),%edi
-	mov    $0x41,%ecx
-	rep stos %eax,%es:(%edi)
-	lea    -0x2415(%ebx),%eax
-	lea    0x258(%esp),%edi
-	mov    %edx,0xc(%esp)
+	call   990 <strlen@plt>
 	mov    %esi,0x8(%esp)
-	mov    %eax,0x4(%esp)
-	mov    %edi,(%esp)
-	call   940 <sprintf@plt>
-	mov    0x24(%esp),%eax
+	add    $0x1,%eax
+	mov    %eax,0xc(%esp)
+	mov    0x40(%esp),%eax
+	mov    %edi,0x4(%esp)
 	mov    %eax,(%esp)
-	call   1330 <get_file_size>
+	call   12f0 <puts@plt+0x780>
+	lea    0x2c(%esp),%esp
+	pop    %ebx
+	pop    %esi
+	pop    %edi
+	pop    %ebp
+	ret
+	mov    %esi,%esi
+	lea    0x0(%edi,%eiz,1),%edi
+	push   %ebx
+	call   114b <puts@plt+0x5db>
+	add    $0x3a9e,%ebx
+	lea    -0x18(%esp),%esp
+	mov    0x24(%esp),%eax
+	movl   $0x0,0x8(%esp)
+	movl   $0xc,(%esp)
+	mov    %eax,0xc(%esp)
+	mov    0x20(%esp),%eax
+	mov    %eax,0x4(%esp)
+	call   970 <ptrace@plt>
 	test   %eax,%eax
-	jne    1248 <load_dex+0x348>
-	call   1910 <get_jni_env>
+	js     14f0 <puts@plt+0x980>
+	xor    %eax,%eax
+	lea    0x18(%esp),%esp
+	pop    %ebx
+	ret
+	lea    -0x1e24(%ebx),%eax
+	mov    %eax,(%esp)
+	call   9a0 <perror@plt>
+	mov    $0xffffffff,%eax
+	jmp    14ea <puts@plt+0x97a>
+	lea    0x0(%esi,%eiz,1),%esi
+	lea    0x0(%edi,%eiz,1),%edi
+	push   %ebx
+	call   114b <puts@plt+0x5db>
+	add    $0x3a3e,%ebx
+	lea    -0x18(%esp),%esp
+	mov    0x24(%esp),%eax
+	movl   $0x0,0x8(%esp)
+	movl   $0xd,(%esp)
 	mov    %eax,0xc(%esp)
-	mov    %eax,%edi
+	mov    0x20(%esp),%eax
+	mov    %eax,0x4(%esp)
+	call   970 <ptrace@plt>
+	test   %eax,%eax
+	js     1550 <puts@plt+0x9e0>
+	xor    %eax,%eax
+	lea    0x18(%esp),%esp
+	pop    %ebx
+	ret
+	lea    -0x1df8(%ebx),%eax
+	mov    %eax,(%esp)
+	call   9a0 <perror@plt>
+	mov    $0xffffffff,%eax
+	jmp    154a <puts@plt+0x9da>
+	lea    0x0(%esi,%eiz,1),%esi
+	lea    0x0(%edi,%eiz,1),%edi
+	push   %ebp
+	push   %edi
+	push   %esi
+	lea    -0x60(%esp),%esp
+	mov    0x70(%esp),%edi
+	lea    0x1c(%esp),%ebp
 	mov    %ebp,0x4(%esp)
-	lea    -0x240f(%ebx),%eax
-	movl   $0x4,(%esp)
-	mov    %eax,0x8(%esp)
-	call   900 <__android_log_print@plt>
-	mov    (%edi),%eax
-	lea    0x48(%esp),%edx
-	mov    %edx,0x4(%esp)
 	mov    %edi,(%esp)
-	call   *0x36c(%eax)
-	test   %eax,%eax
-	jne    12b1 <load_dex+0x3b1>
-	mov    0x48(%esp),%eax
+	call   14b0 <puts@plt+0x940>
+	mov    0x58(%esp),%esi
 	mov    %ebp,0x4(%esp)
-	movl   $0x4,(%esp)
+	mov    %edi,(%esp)
+	sub    0x78(%esp),%esi
+	and    $0xfffffffc,%esi
+	mov    %esi,0x58(%esp)
+	call   1510 <puts@plt+0x9a0>
+	mov    0x78(%esp),%eax
+	mov    %esi,0x4(%esp)
+	mov    %edi,(%esp)
 	mov    %eax,0xc(%esp)
-	lea    -0x23f0(%ebx),%eax
+	mov    0x74(%esp),%eax
 	mov    %eax,0x8(%esp)
-	call   900 <__android_log_print@plt>
-	movl   $0x61c,(%esp)
-	call   960 <malloc@plt>
-	mov    %eax,%edi
-	mov    0x48(%esp),%eax
-	mov    %eax,(%edi)
-	mov    0x2c(%esp),%eax
-	movl   $0x104,0x8(%esp)
+	call   12f0 <puts@plt+0x780>
+	lea    0x60(%esp),%esp
+	mov    %esi,%eax
+	pop    %esi
+	pop    %edi
+	pop    %ebp
+	ret
+	lea    0x0(%esi,%eiz,1),%esi
+	push   %ebx
+	call   114b <puts@plt+0x5db>
+	add    $0x397e,%ebx
+	lea    -0x18(%esp),%esp
+	mov    0x20(%esp),%eax
+	movl   $0x0,0xc(%esp)
+	movl   $0x0,0x8(%esp)
+	movl   $0x7,(%esp)
 	mov    %eax,0x4(%esp)
-	lea    0x4(%edi),%eax
-	mov    %eax,(%esp)
-	call   920 <strncpy@plt>
-	movl   $0x104,0x8(%esp)
-	lea    0x108(%edi),%eax
-	mov    %esi,0x4(%esp)
+	call   970 <ptrace@plt>
+	test   %eax,%eax
+	js     1610 <puts@plt+0xaa0>
+	xor    %eax,%eax
+	lea    0x18(%esp),%esp
+	pop    %ebx
+	ret
+	lea    -0x21b6(%ebx),%eax
 	mov    %eax,(%esp)
-	call   920 <strncpy@plt>
-	mov    0x30(%esp),%eax
-	movl   $0x104,0x8(%esp)
+	call   9a0 <perror@plt>
+	mov    $0xffffffff,%eax
+	jmp    160a <puts@plt+0xa9a>
+	lea    0x0(%esi,%eiz,1),%esi
+	lea    0x0(%edi,%eiz,1),%edi
+	push   %ebp
+	xor    %ebp,%ebp
+	push   %edi
+	push   %esi
+	push   %ebx
+	call   114b <puts@plt+0x5db>
+	add    $0x3919,%ebx
+	lea    -0x3c(%esp),%esp
+	lea    -0x21aa(%ebx),%edi
+	mov    0x5c(%esp),%eax
+	mov    %edi,(%esp)
+	mov    0x50(%esp),%esi
+	mov    %eax,0x8(%esp)
+	mov    0x54(%esp),%eax
 	mov    %eax,0x4(%esp)
-	lea    0x20c(%edi),%eax
-	mov    %eax,(%esp)
-	call   920 <strncpy@plt>
-	mov    0x34(%esp),%eax
-	movl   $0x104,0x8(%esp)
+	call   950 <printf@plt>
+	mov    0x5c(%esp),%eax
+	mov    %edi,0x8(%esp)
+	movl   $0x3,(%esp)
+	mov    %eax,0x10(%esp)
+	mov    0x54(%esp),%eax
+	mov    %eax,0xc(%esp)
+	lea    -0x21da(%ebx),%eax
 	mov    %eax,0x4(%esp)
-	lea    0x310(%edi),%eax
-	mov    %eax,(%esp)
-	call   920 <strncpy@plt>
-	mov    0x38(%esp),%eax
-	movl   $0x104,0x8(%esp)
+	call   960 <__android_log_print@plt>
+	mov    0x5c(%esp),%edx
+	mov    0x58(%esp),%eax
+	test   %edx,%edx
+	lea    -0x4(%eax,%edx,4),%edi
+	je     16d0 <puts@plt+0xb60>
+	jmp    16b0 <puts@plt+0xb40>
+	nop
+	nop
+	nop
+	nop
+	nop
+	nop
+	nop
+	nop
+	nop
+	nop
+	nop
+	nop
+	nop
+	mov    %edi,0x4(%esp)
+	add    $0x1,%ebp
+	movl   $0x4,0x8(%esp)
+	sub    $0x4,%edi
+	mov    %esi,(%esp)
+	call   1570 <puts@plt+0xa00>
+	cmp    0x5c(%esp),%ebp
+	jne    16b0 <puts@plt+0xb40>
+	movl   $0x4,0x8(%esp)
+	lea    0x2c(%esp),%eax
+	mov    %esi,(%esp)
 	mov    %eax,0x4(%esp)
-	lea    0x414(%edi),%eax
-	mov    %eax,(%esp)
-	call   920 <strncpy@plt>
-	mov    0x3c(%esp),%eax
-	movl   $0x104,0x8(%esp)
+	movl   $0x41414140,0x2c(%esp)
+	call   1570 <puts@plt+0xa00>
+	mov    0x60(%esp),%eax
+	mov    %esi,(%esp)
 	mov    %eax,0x4(%esp)
-	lea    0x518(%edi),%eax
-	mov    %eax,(%esp)
-	call   920 <strncpy@plt>
-	mov    %ebp,0x4(%esp)
-	lea    -0x23e5(%ebx),%eax
-	movl   $0x4,(%esp)
-	mov    %eax,0x8(%esp)
-	call   900 <__android_log_print@plt>
-	mov    -0x4(%ebx),%eax
-	mov    %edi,0xc(%esp)
+	call   14b0 <puts@plt+0x940>
+	mov    0x60(%esp),%eax
+	mov    0x54(%esp),%ecx
+	mov    %ecx,0x30(%eax)
+	mov    %eax,0x4(%esp)
+	mov    %esi,(%esp)
+	call   1510 <puts@plt+0x9a0>
+	cmp    $0xffffffff,%eax
+	je     1768 <puts@plt+0xbf8>
+	mov    %esi,(%esp)
+	call   15d0 <puts@plt+0xa60>
+	cmp    $0xffffffff,%eax
+	je     1768 <puts@plt+0xbf8>
+	mov    %esi,(%esp)
+	movl   $0x2,0x8(%esp)
 	movl   $0x0,0x4(%esp)
-	mov    %eax,0x8(%esp)
-	lea    0x4c(%esp),%eax
-	mov    %eax,(%esp)
-	call   970 <pthread_create@plt>
-	xor    %eax,%eax
-	mov    -0x8(%ebx),%edx
-	mov    0x35c(%esp),%ecx
-	mov    (%edx),%edx
-	cmp    %edx,%ecx
-	jne    12d9 <load_dex+0x3d9>
-	lea    0x36c(%esp),%esp
+	call   9b0 <waitpid@plt>
+	mov    0x60(%esp),%eax
+	mov    %esi,(%esp)
+	mov    %eax,0x4(%esp)
+	call   14b0 <puts@plt+0x940>
+	mov    0x60(%esp),%eax
+	mov    0x18(%eax),%eax
+	lea    0x3c(%esp),%esp
 	pop    %ebx
 	pop    %esi
 	pop    %edi
 	pop    %ebp
 	ret
-	nop
-	mov    %edi,(%esp)
-	mov    %eax,0x28(%esp)
-	call   1330 <get_file_size>
-	mov    0x28(%esp),%edx
-	cmp    %eax,%edx
-	je     10c3 <load_dex+0x1c3>
-	movl   $0x1ff,0x4(%esp)
-	mov    %esi,(%esp)
-	call   980 <chmod@plt>
-	mov    0x24(%esp),%eax
-	mov    %edi,0x4(%esp)
-	mov    %eax,(%esp)
-	call   1370 <copyfile>
-	movl   $0x1ff,0x4(%esp)
-	mov    %edi,(%esp)
-	call   980 <chmod@plt>
-	jmp    10c3 <load_dex+0x1c3>
-	lea    0x0(%esi),%esi
-	movl   $0x1ff,0x4(%esp)
-	mov    %esi,(%esp)
-	call   990 <mkdir@plt>
-	mov    0x28(%esp),%edx
-	jmp    107e <load_dex+0x17e>
-	mov    %eax,0xc(%esp)
-	lea    -0x2403(%ebx),%eax
-	mov    %ebp,0x4(%esp)
-	movl   $0x6,(%esp)
-	mov    %eax,0x8(%esp)
-	call   900 <__android_log_print@plt>
+	lea    0x0(%esi,%eiz,1),%esi
+	lea    0x3c(%esp),%esp
 	mov    $0xffffffff,%eax
-	jmp    1224 <load_dex+0x324>
-	call   b70 <dlsym@plt+0xa0>
-	xchg   %ax,%ax
-
-000012e0 <Java_com_test_androidspy_HelperUtil_nativeSetsid>:
-	push   %ebx
-	call   b90 <dlsym@plt+0xc0>
-	add    $0x2c8a,%ebx
-	lea    -0x8(%esp),%esp
-	call   9a0 <setsid@plt>
-	lea    0x8(%esp),%esp
 	pop    %ebx
+	pop    %esi
+	pop    %edi
+	pop    %ebp
 	ret
-	nop
-	lea    0x0(%esi,%eiz,1),%esi
-
-00001300 <Java_com_test_androidspy_HelperUtil_nativeUmask>:
+	lea    0x0(%esi),%esi
+	lea    0x0(%edi,%eiz,1),%edi
 	push   %ebx
-	call   b90 <dlsym@plt+0xc0>
-	add    $0x2c6a,%ebx
+	call   114b <puts@plt+0x5db>
+	add    $0x37ce,%ebx
 	lea    -0x18(%esp),%esp
-	movzwl 0x28(%esp),%eax
-	mov    %eax,(%esp)
-	call   9b0 <umask@plt>
-	lea    0x18(%esp),%esp
+	mov    0x20(%esp),%eax
+	movl   $0x0,0xc(%esp)
+	movl   $0x0,0x8(%esp)
+	movl   $0x11,(%esp)
+	mov    %eax,0x4(%esp)
+	call   970 <ptrace@plt>
+	test   %eax,%eax
+	js     17c0 <puts@plt+0xc50>
 	xor    %eax,%eax
+	lea    0x18(%esp),%esp
 	pop    %ebx
 	ret
+	lea    -0x218f(%ebx),%eax
+	mov    %eax,(%esp)
+	call   9a0 <perror@plt>
+	mov    $0xffffffff,%eax
+	jmp    17ba <puts@plt+0xc4a>
 	lea    0x0(%esi,%eiz,1),%esi
 	lea    0x0(%edi,%eiz,1),%edi
-
-00001330 <get_file_size>:
-	push   %ebx
-	call   b90 <dlsym@plt+0xc0>
-	add    $0x2c3a,%ebx
-	lea    -0x78(%esp),%esp
-	lea    0x10(%esp),%eax
-	mov    %eax,0x4(%esp)
-	mov    0x80(%esp),%eax
-	mov    %eax,(%esp)
-	call   9c0 <stat@plt>
-	test   %eax,%eax
-	mov    $0xffffffff,%edx
-	mov    0x3c(%esp),%eax
-	cmovns %eax,%edx
-	lea    0x78(%esp),%esp
-	pop    %ebx
-	mov    %edx,%eax
-	ret
-	lea    0x0(%esi),%esi
-
-00001370 <copyfile>:
 	push   %ebp
 	push   %edi
 	push   %esi
 	push   %ebx
-	call   b90 <dlsym@plt+0xc0>
-	add    $0x2bf7,%ebx
+	call   114b <puts@plt+0x5db>
+	add    $0x376b,%ebx
 	lea    -0x2c(%esp),%esp
-	lea    -0x250f(%ebx),%ebp
-	mov    0x44(%esp),%eax
-	mov    0x40(%esp),%edi
-	mov    %ebp,0x4(%esp)
-	mov    %eax,0x10(%esp)
-	lea    -0x23cf(%ebx),%eax
+	lea    -0x2164(%ebx),%ebp
+	mov    0x40(%esp),%esi
+	movl   $0x14,0x1c(%esp)
+	movl   $0x0,0x18(%esp)
+	movl   $0x0,0xc(%esp)
+	movl   $0x0,0x8(%esp)
+	mov    %esi,0x4(%esp)
+	movl   $0x10,(%esp)
+	call   970 <ptrace@plt>
+	test   %eax,%eax
+	js     19d8 <puts@plt+0xe68>
+	movl   $0x2,0x8(%esp)
+	movl   $0x0,0x4(%esp)
+	mov    %esi,(%esp)
+	call   9b0 <waitpid@plt>
+	movl   $0x0,0xc(%esp)
+	movl   $0x0,0x8(%esp)
+	mov    %esi,0x4(%esp)
+	movl   $0x18,(%esp)
+	call   970 <ptrace@plt>
+	test   %eax,%eax
+	js     19b8 <puts@plt+0xe48>
+	movl   $0x2,0x8(%esp)
+	movl   $0x0,0x4(%esp)
+	mov    %esi,(%esp)
+	call   9b0 <waitpid@plt>
+	movl   $0x0,0xc(%esp)
+	movl   $0x2c,0x8(%esp)
+	mov    %esi,0x4(%esp)
+	movl   $0x3,(%esp)
+	call   970 <ptrace@plt>
+	mov    %eax,0x4(%esp)
+	mov    %eax,%edi
+	mov    %ebp,(%esp)
+	call   950 <printf@plt>
 	mov    %edi,0xc(%esp)
-	movl   $0x4,(%esp)
-	mov    %eax,0x8(%esp)
-	call   900 <__android_log_print@plt>
-	mov    %edi,(%esp)
-	lea    -0x23c0(%ebx),%eax
+	lea    -0x21da(%ebx),%eax
+	mov    %ebp,0x8(%esp)
+	movl   $0x3,(%esp)
 	mov    %eax,0x4(%esp)
-	call   9d0 <fopen@plt>
+	mov    %eax,0x14(%esp)
+	call   960 <__android_log_print@plt>
+	movl   $0x0,0xc(%esp)
+	movl   $0x0,0x8(%esp)
+	mov    %esi,0x4(%esp)
+	movl   $0x18,(%esp)
+	call   970 <ptrace@plt>
 	test   %eax,%eax
-	mov    %eax,%esi
-	je     1424 <copyfile+0xb4>
-	lea    -0x23ac(%ebx),%eax
+	js     19b8 <puts@plt+0xe48>
+	movl   $0x2,0x8(%esp)
+	movl   $0x0,0x4(%esp)
+	mov    %esi,(%esp)
+	call   9b0 <waitpid@plt>
+	movl   $0x0,0xc(%esp)
+	movl   $0x2c,0x8(%esp)
+	mov    %esi,0x4(%esp)
+	movl   $0x3,(%esp)
+	call   970 <ptrace@plt>
+	mov    %eax,0x4(%esp)
+	mov    %eax,%edi
+	mov    %ebp,(%esp)
+	call   950 <printf@plt>
+	mov    0x14(%esp),%eax
+	mov    %edi,0xc(%esp)
+	mov    %ebp,0x8(%esp)
+	movl   $0x3,(%esp)
 	mov    %eax,0x4(%esp)
+	call   960 <__android_log_print@plt>
 	mov    0x44(%esp),%eax
-	mov    %eax,(%esp)
-	call   9d0 <fopen@plt>
 	test   %eax,%eax
-	mov    %eax,%edi
-	jne    13fc <copyfile+0x8c>
-	jmp    1449 <copyfile+0xd9>
-	lea    0x0(%esi,%eiz,1),%esi
-	mov    %edi,0x4(%esp)
-	mov    %eax,(%esp)
-	call   9e0 <fputc@plt>
-	mov    %esi,(%esp)
-	call   9f0 <getc@plt>
-	cmp    $0xffffffff,%eax
-	jne    13f0 <copyfile+0x80>
+	je     1990 <puts@plt+0xe20>
+	cmp    %edi,0x10c(%ebx)
+	je     1998 <puts@plt+0xe28>
 	mov    %esi,(%esp)
-	call   a00 <fclose@plt>
-	mov    %edi,(%esp)
-	call   a00 <fclose@plt>
+	call   1780 <puts@plt+0xc10>
+	subl   $0x1,0x1c(%esp)
+	je     19d0 <puts@plt+0xe60>
+	mov    %edi,0x18(%esp)
+	jmp    180d <puts@plt+0xc9d>
+	nop
+	cmp    %edi,0x10c(%ebx)
+	jne    19a6 <puts@plt+0xe36>
+	mov    0x18(%esp),%eax
+	sub    $0xf0,%eax
+	cmp    $0x1,%eax
+	jbe    1977 <puts@plt+0xe07>
 	xor    %eax,%eax
 	lea    0x2c(%esp),%esp
 	pop    %ebx
 	pop    %esi
 	pop    %edi
 	pop    %ebp
 	ret
-	mov    %edi,0xc(%esp)
-	mov    %ebp,0x4(%esp)
-	lea    -0x23bd(%ebx),%eax
-	movl   $0x6,(%esp)
-	mov    %eax,0x8(%esp)
-	call   900 <__android_log_print@plt>
+	lea    0x0(%esi,%eiz,1),%esi
+	lea    -0x2173(%ebx),%eax
+	mov    %eax,(%esp)
+	call   9a0 <perror@plt>
 	mov    $0xffffffff,%eax
-	jmp    141b <copyfile+0xab>
-	mov    0x44(%esp),%eax
-	mov    %eax,0xc(%esp)
-	jmp    1428 <copyfile+0xb8>
+	jmp    19a8 <puts@plt+0xe38>
+	lea    0x0(%esi),%esi
+	mov    $0xffffffff,%eax
+	jmp    19a8 <puts@plt+0xe38>
+	nop
+	lea    -0x2181(%ebx),%eax
+	mov    %eax,(%esp)
+	call   9a0 <perror@plt>
+	mov    $0xffffffff,%eax
+	jmp    19a8 <puts@plt+0xe38>
 	lea    0x0(%esi),%esi
-	lea    0x0(%edi,%eiz,1),%edi
-
-00001460 <get_module_base>:
 	push   %ebp
 	push   %edi
 	push   %esi
 	push   %ebx
-	call   b90 <dlsym@plt+0xc0>
-	add    $0x2b07,%ebx
-	lea    -0x42c(%esp),%esp
-	mov    -0x8(%ebx),%eax
+	call   114b <puts@plt+0x5db>
+	add    $0x355b,%ebx
+	lea    -0x44c(%esp),%esp
+	mov    -0x10(%ebx),%ecx
+	mov    0x460(%esp),%eax
+	mov    0x464(%esp),%ebp
+	mov    (%ecx),%edx
+	test   %eax,%eax
+	mov    %edx,0x43c(%esp)
+	js     1b00 <puts@plt+0xf90>
+	mov    %eax,0xc(%esp)
 	lea    0x1c(%esp),%esi
-	mov    0x440(%esp),%ebp
-	mov    (%eax),%eax
-	mov    %eax,0x41c(%esp)
-	lea    -0x23a9(%ebx),%eax
+	movl   $0x20,0x4(%esp)
+	lea    -0x214b(%ebx),%eax
+	mov    %esi,(%esp)
+	mov    %eax,0x8(%esp)
+	call   9c0 <snprintf@plt>
+	mov    %esi,(%esp)
+	lea    -0x213d(%ebx),%eax
 	mov    %eax,0x4(%esp)
-	lea    -0x23a7(%ebx),%eax
-	mov    %eax,(%esp)
+	lea    0x3c(%esp),%esi
 	call   9d0 <fopen@plt>
 	test   %eax,%eax
 	mov    %eax,%edi
-	jne    14c8 <get_module_base+0x68>
-	jmp    1545 <get_module_base+0xe5>
-	nop
-	lea    0x0(%esi,%eiz,1),%esi
+	jne    1a80 <puts@plt+0xf10>
+	jmp    1b29 <puts@plt+0xfb9>
+	xchg   %ax,%ax
 	mov    %ebp,0x4(%esp)
 	mov    %esi,(%esp)
-	call   a10 <strstr@plt>
+	call   9e0 <strstr@plt>
 	test   %eax,%eax
-	jne    1510 <get_module_base+0xb0>
+	jne    1ac8 <puts@plt+0xf58>
 	mov    %edi,0x8(%esp)
 	movl   $0x400,0x4(%esp)
 	mov    %esi,(%esp)
-	call   a20 <fgets@plt>
+	call   9f0 <fgets@plt>
 	test   %eax,%eax
-	jne    14b8 <get_module_base+0x58>
+	jne    1a70 <puts@plt+0xf00>
 	xor    %esi,%esi
 	mov    %edi,(%esp)
 	call   a00 <fclose@plt>
-	mov    -0x8(%ebx),%edx
+	mov    -0x10(%ebx),%edx
 	mov    %esi,%eax
-	mov    0x41c(%esp),%ecx
+	mov    0x43c(%esp),%ecx
 	mov    (%edx),%edx
 	cmp    %edx,%ecx
-	jne    1549 <get_module_base+0xe9>
-	lea    0x42c(%esp),%esp
+	jne    1b30 <puts@plt+0xfc0>
+	lea    0x44c(%esp),%esp
 	pop    %ebx
 	pop    %esi
 	pop    %edi
 	pop    %ebp
 	ret
 	nop
 	lea    0x0(%esi,%eiz,1),%esi
 	mov    %esi,(%esp)
-	lea    -0x2397(%ebx),%eax
+	lea    -0x213b(%ebx),%eax
 	mov    %eax,0x4(%esp)
-	call   a30 <strtok@plt>
+	call   a10 <strtok@plt>
 	mov    %eax,(%esp)
 	movl   $0x10,0x8(%esp)
 	movl   $0x0,0x4(%esp)
-	call   a40 <strtoul@plt>
+	call   a20 <strtoul@plt>
 	cmp    $0x8000,%eax
 	mov    %eax,%esi
-	jne    14e2 <get_module_base+0x82>
-	jmp    14e0 <get_module_base+0x80>
+	jne    1a9a <puts@plt+0xf2a>
+	jmp    1a98 <puts@plt+0xf28>
+	lea    0x0(%esi),%esi
+	movl   $0x6f72702f,0x1c(%esp)
+	lea    0x1c(%esp),%esi
+	movl   $0x65732f63,0x20(%esp)
+	movl   $0x6d2f666c,0x24(%esp)
+	movl   $0x737061,0x28(%esp)
+	jmp    1a4d <puts@plt+0xedd>
 	xor    %esi,%esi
-	jmp    14ea <get_module_base+0x8a>
-	lea    0x0(%esi,%eiz,1),%esi
-	call   b70 <dlsym@plt+0xa0>
+	jmp    1aa2 <puts@plt+0xf32>
+	call   1130 <puts@plt+0x5c0>
 	lea    0x0(%esi,%eiz,1),%esi
 	lea    0x0(%edi,%eiz,1),%edi
-
-00001560 <get_symbol_offset>:
+	push   %edi
+	push   %esi
+	lea    -0x14(%esp),%esp
+	mov    0x24(%esp),%esi
+	movl   $0xffffffff,(%esp)
+	mov    %esi,0x4(%esp)
+	call   19f0 <puts@plt+0xe80>
+	mov    %esi,0x4(%esp)
+	mov    %eax,%edi
+	mov    0x20(%esp),%eax
+	mov    %eax,(%esp)
+	call   19f0 <puts@plt+0xe80>
+	add    0x28(%esp),%eax
+	lea    0x14(%esp),%esp
+	pop    %esi
+	sub    %edi,%eax
+	pop    %edi
+	ret
+	lea    0x0(%esi,%eiz,1),%esi
 	push   %ebp
 	push   %edi
 	push   %esi
 	push   %ebx
-	call   b90 <dlsym@plt+0xc0>
-	add    $0x2a07,%ebx
-	lea    -0xac(%esp),%esp
-	mov    0xc0(%esp),%ebp
+	call   114b <puts@plt+0x5db>
+	add    $0x33cb,%ebx
+	lea    -0x9c(%esp),%esp
+	mov    0xb0(%esp),%edi
 	movl   $0x0,0x4(%esp)
-	mov    %ebp,(%esp)
-	call   a50 <open@plt>
+	mov    %edi,(%esp)
+	call   a30 <open@plt>
 	cmp    $0xffffffff,%eax
 	mov    %eax,%esi
-	je     1898 <get_symbol_offset+0x338>
-	xor    %eax,%eax
-	lea    0x40(%esp),%edi
-	mov    $0x18,%ecx
-	rep stos %eax,%es:(%edi)
+	je     1def <puts@plt+0x127f>
 	mov    %esi,(%esp)
-	lea    0x40(%esp),%eax
-	mov    %eax,0x4(%esp)
-	call   a60 <fstat@plt>
-	test   %eax,%eax
-	jne    17c0 <get_symbol_offset+0x260>
-	mov    0x6c(%esp),%eax
-	mov    %ebp,0xc(%esp)
-	movl   $0x3,(%esp)
-	mov    %eax,0x34(%esp)
-	mov    %eax,%edi
-	mov    %eax,0x10(%esp)
-	lea    -0x2370(%ebx),%eax
-	mov    %eax,0x8(%esp)
-	lea    -0x250f(%ebx),%eax
+	lea    0x30(%esp),%eax
 	mov    %eax,0x4(%esp)
-	mov    %eax,0x38(%esp)
-	call   900 <__android_log_print@plt>
-	movl   $0x0,0x14(%esp)
-	movl   $0x0,0x10(%esp)
-	movl   $0x22,0xc(%esp)
-	movl   $0x3,0x8(%esp)
-	mov    %edi,0x4(%esp)
-	movl   $0x0,(%esp)
-	call   a70 <mmap@plt>
-	mov    %eax,0x2c(%esp)
-	cmp    $0xffffffff,%eax
-	je     18ca <get_symbol_offset+0x36a>
-	mov    0x2c(%esp),%edi
-	mov    0x34(%esp),%ebp
-	movl   $0x0,0x4(%esp)
+	call   a40 <fstat@plt>
+	mov    0x5c(%esp),%edi
 	mov    %edi,(%esp)
-	mov    %ebp,0x8(%esp)
-	call   a80 <memset@plt>
-	mov    %ebp,0x8(%esp)
-	mov    %edi,0x4(%esp)
+	call   a50 <malloc@plt>
+	mov    %eax,(%esp)
+	mov    %eax,%ebp
+	mov    %edi,0x8(%esp)
+	movl   $0x0,0x4(%esp)
+	mov    %eax,0x24(%esp)
+	call   a60 <memset@plt>
+	mov    %edi,0x8(%esp)
+	mov    %ebp,0x4(%esp)
 	mov    %esi,(%esp)
-	call   a90 <read@plt>
+	call   a70 <read@plt>
 	mov    %esi,(%esp)
-	call   aa0 <close@plt>
-	mov    0x20(%edi),%ecx
-	movzwl 0x2e(%edi),%eax
-	add    %edi,%ecx
-	test   %ax,%ax
-	je     18ef <get_symbol_offset+0x38f>
-	lea    (%eax,%eax,4),%eax
+	call   a80 <close@plt>
+	mov    0x20(%ebp),%ecx
+	movzwl 0x2e(%ebp),%edi
+	add    %ebp,%ecx
+	test   %edi,%edi
+	je     1e38 <puts@plt+0x12c8>
+	mov    0x4(%ecx),%eax
 	xor    %esi,%esi
-	movl   $0x0,0x3c(%esp)
-	xor    %edi,%edi
-	shl    $0x3,%eax
-	movl   $0x0,0x30(%esp)
 	movl   $0x0,0x20(%esp)
 	movl   $0x0,0x28(%esp)
-	mov    %eax,0x24(%esp)
-	jmp    16d4 <get_symbol_offset+0x174>
+	movl   $0x0,0x2c(%esp)
+	movl   $0x0,0x1c(%esp)
+	jmp    1c75 <puts@plt+0x1105>
 	xchg   %ax,%ax
 	mov    0x10(%ecx),%eax
 	xor    %edx,%edx
-	mov    %eax,0x28(%esp)
+	mov    %eax,0x20(%esp)
 	mov    0x14(%ecx),%eax
 	divl   0x24(%ecx)
-	mov    %eax,0x20(%esp)
+	mov    %eax,0x1c(%esp)
 	mov    %ebp,%eax
 	test   %al,%al
-	jne    17f8 <get_symbol_offset+0x298>
-	add    $0x28,%esi
-	add    $0x1,%edi
+	jne    1d58 <puts@plt+0x11e8>
+	add    $0x1,%esi
+	cmp    %edi,%esi
+	jge    1cb0 <puts@plt+0x1140>
+	mov    0x28(%ecx),%ebp
+	mov    0x2c(%ecx),%eax
+	test   %ebp,%ebp
+	jne    1c72 <puts@plt+0x1102>
+	test   %eax,%eax
+	je     1cb0 <puts@plt+0x1140>
 	add    $0x28,%ecx
-	cmp    0x24(%esp),%esi
-	je     1710 <get_symbol_offset+0x1b0>
-	mov    0x4(%ecx),%eax
 	cmp    $0xb,%eax
 	sete   %dl
 	mov    %edx,%ebp
-	je     16a8 <get_symbol_offset+0x148>
+	je     1c40 <puts@plt+0x10d0>
 	cmp    $0x2,%eax
-	je     16a8 <get_symbol_offset+0x148>
+	je     1c40 <puts@plt+0x10d0>
 	cmp    $0x3,%eax
-	jne    16c5 <get_symbol_offset+0x165>
-	mov    0x2c(%esp),%eax
+	jne    1c5d <puts@plt+0x10ed>
+	mov    0x24(%esp),%eax
 	movzwl 0x32(%eax),%eax
-	cmp    %edi,%eax
-	je     16c5 <get_symbol_offset+0x165>
-	add    $0x28,%esi
-	add    $0x1,%edi
+	cmp    %esi,%eax
+	je     1c5d <puts@plt+0x10ed>
 	mov    0x10(%ecx),%eax
-	add    $0x28,%ecx
-	cmp    0x24(%esp),%esi
-	mov    %eax,0x30(%esp)
-	jne    16d4 <get_symbol_offset+0x174>
+	add    $0x1,%esi
+	cmp    %edi,%esi
+	mov    %eax,0x28(%esp)
+	jl     1c64 <puts@plt+0x10f4>
 	lea    0x0(%esi),%esi
-	mov    0x28(%esp),%ecx
-	mov    0x30(%esp),%esi
+	lea    0x0(%edi,%eiz,1),%edi
+	mov    0x20(%esp),%ecx
+	mov    0x28(%esp),%eax
 	test   %ecx,%ecx
-	mov    %esi,%eax
-	je     183d <get_symbol_offset+0x2dd>
-	mov    0x20(%esp),%edx
+	je     1d9d <puts@plt+0x122d>
+	mov    0x1c(%esp),%edx
 	test   %edx,%edx
-	je     183d <get_symbol_offset+0x2dd>
-	test   %esi,%esi
-	je     1841 <get_symbol_offset+0x2e1>
-	mov    0x2c(%esp),%eax
-	mov    0x28(%esp),%edi
-	mov    0x30(%esp),%esi
+	je     1d9d <puts@plt+0x122d>
+	mov    0x28(%esp),%edx
+	test   %edx,%edx
+	je     1da1 <puts@plt+0x1231>
+	mov    0x24(%esp),%eax
+	mov    0x20(%esp),%edi
+	mov    0x28(%esp),%esi
 	add    %eax,%edi
 	add    %eax,%esi
-	mov    0x20(%esp),%eax
+	mov    0x1c(%esp),%eax
 	test   %eax,%eax
-	jle    1873 <get_symbol_offset+0x313>
+	jle    1e1e <puts@plt+0x12ae>
 	xor    %ebp,%ebp
 	mov    %edi,%eax
 	mov    %ebp,%edi
 	mov    %eax,%ebp
-	jmp    1770 <get_symbol_offset+0x210>
-	lea    0x0(%esi,%eiz,1),%esi
+	jmp    1d10 <puts@plt+0x11a0>
+	xchg   %ax,%ax
 	add    $0x1,%edi
 	add    $0x10,%ebp
-	cmp    0x20(%esp),%edi
-	je     1873 <get_symbol_offset+0x313>
-	mov    0xc4(%esp),%eax
+	cmp    0x1c(%esp),%edi
+	je     1e1e <puts@plt+0x12ae>
+	mov    0xb4(%esp),%eax
 	mov    %eax,0x4(%esp)
 	mov    0x0(%ebp),%eax
 	add    %esi,%eax
 	mov    %eax,(%esp)
-	call   ab0 <strcmp@plt>
+	call   a90 <strcmp@plt>
 	test   %eax,%eax
-	jne    1760 <get_symbol_offset+0x200>
-	mov    0x34(%esp),%eax
+	jne    1d00 <puts@plt+0x1190>
+	mov    0x24(%esp),%eax
 	mov    0x4(%ebp),%esi
-	mov    %eax,0x4(%esp)
-	mov    0x2c(%esp),%eax
 	mov    %eax,(%esp)
-	call   ac0 <munmap@plt>
+	call   aa0 <free@plt>
 	test   %esi,%esi
-	je     1887 <get_symbol_offset+0x327>
+	je     1e2a <puts@plt+0x12ba>
 	mov    %esi,%eax
-	sub    0x3c(%esp),%eax
-	lea    0xac(%esp),%esp
+	sub    0x2c(%esp),%eax
+	lea    0x9c(%esp),%esp
 	pop    %ebx
 	pop    %esi
 	pop    %edi
 	pop    %ebp
 	ret
 	lea    0x0(%esi),%esi
-	mov    %eax,0x10(%esp)
-	lea    -0x2384(%ebx),%eax
-	mov    %eax,0x8(%esp)
-	lea    -0x250f(%ebx),%eax
-	mov    %ebp,0xc(%esp)
-	movl   $0x6,(%esp)
-	mov    %eax,0x4(%esp)
-	call   900 <__android_log_print@plt>
-	xor    %eax,%eax
-	lea    0xac(%esp),%esp
-	pop    %ebx
-	pop    %esi
-	pop    %edi
-	pop    %ebp
-	ret
-	xchg   %ax,%ax
-	mov    0x2c(%esp),%edx
+	mov    0x24(%esp),%edx
 	mov    0x1c(%edx),%eax
 	movzwl 0x2c(%edx),%ebp
 	add    %edx,%eax
 	test   %bp,%bp
-	je     16c5 <get_symbol_offset+0x165>
+	je     1c5d <puts@plt+0x10ed>
 	add    $0x1,%ebp
 	mov    $0x1,%edx
-	jmp    1826 <get_symbol_offset+0x2c6>
+	jmp    1d86 <puts@plt+0x1216>
 	add    $0x1,%edx
 	add    $0x20,%eax
 	cmp    %ebp,%edx
-	je     16c5 <get_symbol_offset+0x165>
+	je     1c5d <puts@plt+0x10ed>
 	cmpl   $0x1,(%eax)
-	jne    1818 <get_symbol_offset+0x2b8>
+	jne    1d78 <puts@plt+0x1208>
 	cmpl   $0x0,0x4(%eax)
-	jne    1818 <get_symbol_offset+0x2b8>
+	jne    1d78 <puts@plt+0x1208>
 	mov    0x8(%eax),%eax
-	mov    %eax,0x3c(%esp)
-	jmp    16c5 <get_symbol_offset+0x165>
-	mov    0x30(%esp),%eax
+	mov    %eax,0x2c(%esp)
+	jmp    1c5d <puts@plt+0x10ed>
+	mov    0x28(%esp),%eax
 	mov    %eax,0x14(%esp)
-	mov    0x20(%esp),%eax
+	mov    0x1c(%esp),%eax
 	movl   $0x6,(%esp)
 	mov    %eax,0x10(%esp)
-	mov    0x28(%esp),%eax
+	mov    0x20(%esp),%eax
 	mov    %eax,0xc(%esp)
-	lea    -0x224c(%ebx),%eax
+	lea    -0x1dcc(%ebx),%eax
 	mov    %eax,0x8(%esp)
-	mov    0x38(%esp),%eax
+	lea    -0x21da(%ebx),%eax
 	mov    %eax,0x4(%esp)
-	call   900 <__android_log_print@plt>
-	mov    0x34(%esp),%eax
-	mov    %eax,0x4(%esp)
-	mov    0x2c(%esp),%eax
+	call   960 <__android_log_print@plt>
+	mov    0x24(%esp),%eax
 	mov    %eax,(%esp)
-	call   ac0 <munmap@plt>
-	lea    0xac(%esp),%esp
+	call   aa0 <free@plt>
+	lea    0x9c(%esp),%esp
 	xor    %eax,%eax
 	pop    %ebx
 	pop    %esi
 	pop    %edi
 	pop    %ebp
 	ret
-	lea    0x0(%esi),%esi
-	mov    %ebp,0xc(%esp)
-	lea    -0x2395(%ebx),%eax
-	mov    %eax,0x8(%esp)
-	lea    -0x250f(%ebx),%eax
-	movl   $0x6,(%esp)
+	mov    %edi,0x8(%esp)
+	lea    -0x2139(%ebx),%eax
 	mov    %eax,0x4(%esp)
-	call   900 <__android_log_print@plt>
-	lea    0xac(%esp),%esp
+	mov    -0xc(%ebx),%eax
+	add    $0xa8,%eax
+	mov    %eax,(%esp)
+	call   ab0 <fprintf@plt>
+	lea    0x9c(%esp),%esp
 	xor    %eax,%eax
 	pop    %ebx
 	pop    %esi
 	pop    %edi
 	pop    %ebp
 	ret
-	movl   $0x6,(%esp)
-	lea    -0x2364(%ebx),%eax
-	mov    %eax,0x8(%esp)
-	mov    0x38(%esp),%eax
-	mov    %eax,0x4(%esp)
-	call   900 <__android_log_print@plt>
+	mov    0x24(%esp),%eax
+	mov    %eax,(%esp)
+	call   aa0 <free@plt>
+	lea    0x9c(%esp),%esp
 	xor    %eax,%eax
-	jmp    17ea <get_symbol_offset+0x28a>
-	movl   $0x0,0x20(%esp)
+	pop    %ebx
+	pop    %esi
+	pop    %edi
+	pop    %ebp
+	ret
+	movl   $0x0,0x1c(%esp)
 	xor    %eax,%eax
-	movl   $0x0,0x28(%esp)
-	jmp    1841 <get_symbol_offset+0x2e1>
-	lea    0x0(%esi),%esi
-	lea    0x0(%edi,%eiz,1),%edi
-
-00001910 <get_jni_env>:
+	movl   $0x0,0x20(%esp)
+	jmp    1da1 <puts@plt+0x1231>
+	nop
 	push   %ebp
 	push   %edi
 	push   %esi
 	push   %ebx
-	call   b90 <dlsym@plt+0xc0>
-	add    $0x2657,%ebx
+	call   114b <puts@plt+0x5db>
+	add    $0x30fb,%ebx
 	lea    -0x2c(%esp),%esp
-	lea    -0x2210(%ebx),%esi
-	mov    %esi,0x4(%esp)
-	movl   $0xffffffff,(%esp)
+	lea    -0x2128(%ebx),%ebp
+	mov    0x40(%esp),%edi
+	call   1150 <puts@plt+0x5e0>
+	mov    %eax,0x4(%esp)
+	mov    %eax,%esi
+	mov    %ebp,(%esp)
+	call   950 <printf@plt>
+	mov    %ebp,0x8(%esp)
+	lea    -0x21da(%ebx),%ebp
+	mov    %esi,0xc(%esp)
+	movl   $0x3,(%esp)
+	mov    %ebp,0x4(%esp)
+	call   960 <__android_log_print@plt>
+	cmp    $0x1c,%esi
+	jle    1eb9 <puts@plt+0x1349>
+	mov    %edi,(%esp)
+	lea    0x22c(%ebx),%eax
+	mov    %eax,0x4(%esp)
+	call   a90 <strcmp@plt>
+	test   %eax,%eax
+	je     1ee8 <puts@plt+0x1378>
+	movl   $0x0,0x4(%esp)
+	mov    %edi,(%esp)
+	call   ac0 <dlopen@plt>
+	mov    0x44(%esp),%ecx
+	mov    %eax,(%esp)
+	mov    %ecx,0x4(%esp)
 	call   ad0 <dlsym@plt>
 	test   %eax,%eax
-	mov    %eax,%edi
-	je     1970 <get_jni_env+0x60>
-	mov    %eax,0xc(%esp)
-	lea    -0x2350(%ebx),%eax
-	mov    %eax,0x8(%esp)
-	lea    -0x250f(%ebx),%eax
-	movl   $0x4,(%esp)
-	mov    %eax,0x4(%esp)
-	call   900 <__android_log_print@plt>
-	call   *%edi
+	je     1ee8 <puts@plt+0x1378>
 	lea    0x2c(%esp),%esp
 	pop    %ebx
 	pop    %esi
 	pop    %edi
 	pop    %ebp
 	ret
 	xchg   %ax,%ax
-	lea    -0x21e8(%ebx),%edi
+	mov    0x44(%esp),%eax
 	mov    %edi,(%esp)
-	call   1460 <get_module_base>
-	mov    %eax,0x10(%esp)
+	mov    %eax,0x4(%esp)
+	call   1b80 <puts@plt+0x1010>
+	lea    -0x2113(%ebx),%edx
+	mov    %eax,%esi
+	mov    %eax,0x4(%esp)
+	mov    %edx,(%esp)
+	mov    %edx,0x1c(%esp)
+	call   950 <printf@plt>
+	mov    0x1c(%esp),%edx
+	mov    %esi,0xc(%esp)
+	mov    %ebp,0x4(%esp)
+	movl   $0x3,(%esp)
+	mov    %edx,0x8(%esp)
+	call   960 <__android_log_print@plt>
+	xor    %eax,%eax
+	test   %esi,%esi
+	je     1edd <puts@plt+0x136d>
+	mov    %edi,0x4(%esp)
+	movl   $0xffffffff,(%esp)
+	call   19f0 <puts@plt+0xe80>
+	lea    0x2c(%esp),%esp
+	add    %esi,%eax
+	pop    %ebx
+	pop    %esi
+	pop    %edi
+	pop    %ebp
+	ret
+	lea    0x0(%esi),%esi
+	push   %ebp
+	push   %edi
+	push   %esi
+	push   %ebx
+	call   114b <puts@plt+0x5db>
+	add    $0x2ffb,%ebx
+	lea    -0x15c(%esp),%esp
+	mov    -0x10(%ebx),%eax
+	mov    0x170(%esp),%edi
+	mov    (%eax),%eax
+	test   %edi,%edi
+	mov    %eax,0x14c(%esp)
+	je     2078 <puts@plt+0x1508>
+	lea    -0x2109(%ebx),%eax
+	mov    %eax,(%esp)
+	call   ae0 <opendir@plt>
+	test   %eax,%eax
+	mov    %eax,%esi
+	je     2078 <puts@plt+0x1508>
+	lea    -0x2103(%ebx),%eax
+	mov    %eax,0x14(%esp)
+	jmp    1fb9 <puts@plt+0x1449>
+	add    $0x13,%eax
+	mov    %eax,(%esp)
+	call   940 <atoi@plt>
+	test   %eax,%eax
 	mov    %eax,%ebp
-	mov    %edi,0xc(%esp)
-	lea    -0x2339(%ebx),%eax
+	jne    1ff8 <puts@plt+0x1488>
+	mov    %esi,(%esp)
+	call   af0 <readdir@plt>
+	test   %eax,%eax
+	jne    1fa8 <puts@plt+0x1438>
+	mov    $0xffffffff,%ebp
+	mov    %esi,(%esp)
+	call   b00 <closedir@plt>
+	mov    %ebp,%eax
+	mov    -0x10(%ebx),%edi
+	mov    0x14c(%esp),%ecx
+	mov    (%edi),%edx
+	cmp    %edx,%ecx
+	jne    2085 <puts@plt+0x1515>
+	lea    0x15c(%esp),%esp
+	pop    %ebx
+	pop    %esi
+	pop    %edi
+	pop    %ebp
+	ret
+	nop
 	mov    %eax,0x8(%esp)
-	lea    -0x250f(%ebx),%eax
-	movl   $0x4,(%esp)
+	lea    0x2c(%esp),%edx
+	mov    0x14(%esp),%eax
+	mov    %edx,(%esp)
+	mov    %edx,0x18(%esp)
 	mov    %eax,0x4(%esp)
-	mov    %eax,0x18(%esp)
-	call   900 <__android_log_print@plt>
-	test   %ebp,%ebp
-	je     1a2d <get_jni_env+0x11d>
+	call   b10 <sprintf@plt>
+	mov    0x18(%esp),%edx
+	lea    -0x213d(%ebx),%eax
+	mov    %eax,0x4(%esp)
+	mov    %edx,(%esp)
+	call   9d0 <fopen@plt>
+	test   %eax,%eax
+	je     1fb9 <puts@plt+0x1449>
+	mov    %eax,0x8(%esp)
+	lea    0x4c(%esp),%ecx
+	movl   $0x100,0x4(%esp)
+	mov    %ecx,(%esp)
+	mov    %eax,0x1c(%esp)
+	mov    %ecx,0x18(%esp)
+	call   9f0 <fgets@plt>
+	mov    0x1c(%esp),%edx
+	mov    %edx,(%esp)
+	call   a00 <fclose@plt>
+	mov    0x18(%esp),%ecx
+	mov    %edi,(%esp)
+	mov    %ecx,0x4(%esp)
+	call   a90 <strcmp@plt>
+	test   %eax,%eax
+	jne    1fb9 <puts@plt+0x1449>
+	jmp    1fca <puts@plt+0x145a>
+	nop
+	mov    $0xffffffff,%eax
+	lea    0x0(%esi),%esi
+	jmp    1fd4 <puts@plt+0x1464>
+	call   1130 <puts@plt+0x5c0>
+	lea    0x0(%esi),%esi
+	push   %ebp
+	push   %edi
+	push   %esi
+	push   %ebx
+	call   114b <puts@plt+0x5db>
+	add    $0x2ebb,%ebx
+	lea    -0x5c(%esp),%esp
+	lea    0x32c(%ebx),%edi
+	lea    -0x20f2(%ebx),%eax
+	lea    -0x20ed(%ebx),%esi
+	mov    %edi,(%esp)
+	mov    %eax,0x4(%esp)
+	call   1e50 <puts@plt+0x12e0>
+	mov    %eax,0x8(%esp)
+	mov    %eax,0x1c(%esp)
+	mov    0x70(%esp),%eax
+	mov    %edi,0x4(%esp)
+	mov    %eax,(%esp)
+	call   1b40 <puts@plt+0xfd0>
+	mov    %esi,(%esp)
+	mov    %eax,%ebp
+	mov    0x74(%esp),%eax
+	mov    %eax,0x4(%esp)
+	call   950 <printf@plt>
+	mov    0x74(%esp),%eax
+	mov    %esi,0x8(%esp)
+	lea    -0x21da(%ebx),%esi
+	movl   $0x3,(%esp)
+	mov    %eax,0xc(%esp)
 	mov    %esi,0x4(%esp)
+	call   960 <__android_log_print@plt>
+	mov    %edi,0x4(%esp)
+	lea    -0x20d3(%ebx),%ecx
+	mov    %ecx,(%esp)
+	mov    %ecx,0x18(%esp)
+	call   950 <printf@plt>
+	mov    0x18(%esp),%ecx
+	mov    %edi,0xc(%esp)
+	lea    -0x20c0(%ebx),%edi
+	mov    %esi,0x4(%esp)
+	movl   $0x3,(%esp)
+	mov    %ecx,0x8(%esp)
+	call   960 <__android_log_print@plt>
+	mov    0x1c(%esp),%edx
+	mov    %edi,(%esp)
+	mov    %edx,0x4(%esp)
+	mov    %edx,0x18(%esp)
+	call   950 <printf@plt>
+	mov    0x18(%esp),%edx
+	mov    %edi,0x8(%esp)
+	lea    -0x20a7(%ebx),%edi
+	mov    %esi,0x4(%esp)
+	movl   $0x3,(%esp)
+	mov    %edx,0xc(%esp)
+	call   960 <__android_log_print@plt>
+	mov    %ebp,0x4(%esp)
 	mov    %edi,(%esp)
-	call   1560 <get_symbol_offset>
+	call   950 <printf@plt>
+	mov    %ebp,0xc(%esp)
+	mov    %edi,0x8(%esp)
+	lea    -0x1d90(%ebx),%edi
+	mov    %esi,0x4(%esp)
+	movl   $0x3,(%esp)
+	call   960 <__android_log_print@plt>
+	mov    0x74(%esp),%eax
+	mov    %edi,(%esp)
+	movl   $0x0,0x28(%esp)
+	mov    %eax,0x2c(%esp)
+	mov    0x70(%esp),%eax
+	movl   $0x3,0x30(%esp)
+	movl   $0x22,0x34(%esp)
+	mov    %eax,0x4(%esp)
+	movl   $0x0,0x38(%esp)
+	movl   $0x0,0x3c(%esp)
+	call   950 <printf@plt>
+	mov    0x70(%esp),%eax
+	mov    %edi,0x8(%esp)
+	mov    %esi,0x4(%esp)
+	movl   $0x3,(%esp)
+	mov    %eax,0xc(%esp)
+	call   960 <__android_log_print@plt>
+	mov    0x78(%esp),%eax
+	mov    %ebp,0x4(%esp)
+	lea    -0x208d(%ebx),%ebp
+	movl   $0x6,0xc(%esp)
 	mov    %eax,0x10(%esp)
-	mov    %eax,0x1c(%esp)
-	lea    -0x2326(%ebx),%eax
+	lea    0x28(%esp),%eax
 	mov    %eax,0x8(%esp)
-	mov    0x18(%esp),%eax
+	mov    0x70(%esp),%eax
+	mov    %eax,(%esp)
+	call   1630 <puts@plt+0xac0>
+	mov    %eax,0x4(%esp)
+	mov    %eax,%edi
+	mov    %ebp,(%esp)
+	call   950 <printf@plt>
+	mov    %edi,0xc(%esp)
+	mov    %ebp,0x8(%esp)
+	mov    %esi,0x4(%esp)
+	movl   $0x3,(%esp)
+	call   960 <__android_log_print@plt>
+	lea    0x5c(%esp),%esp
+	mov    %edi,%eax
+	pop    %ebx
+	pop    %esi
+	pop    %edi
+	pop    %ebp
+	ret
+	push   %ebp
+	push   %edi
+	push   %esi
+	push   %ebx
+	call   114b <puts@plt+0x5db>
+	add    $0x2ceb,%ebx
+	lea    -0x7c(%esp),%esp
+	lea    0x32c(%ebx),%edi
+	mov    %edi,(%esp)
+	lea    0x2c(%esp),%ebp
+	movl   $0x0,0x4(%esp)
+	mov    0x90(%esp),%esi
+	call   ac0 <dlopen@plt>
+	mov    %eax,(%esp)
+	lea    -0x2073(%ebx),%edx
+	mov    %edx,0x4(%esp)
+	call   ad0 <dlsym@plt>
+	mov    %eax,0x8(%esp)
+	mov    %edi,0x4(%esp)
+	mov    %esi,(%esp)
+	call   1b40 <puts@plt+0xfd0>
+	mov    %ebp,0x4(%esp)
+	mov    %eax,%edi
+	mov    %esi,(%esp)
+	call   14b0 <puts@plt+0x940>
+	cmp    $0xffffffff,%eax
+	je     2343 <puts@plt+0x17d3>
+	mov    %ebp,0x10(%esp)
+	lea    -0x206b(%ebx),%ebp
+	mov    %edi,0x4(%esp)
+	movl   $0x0,0xc(%esp)
+	movl   $0x0,0x8(%esp)
+	mov    %esi,(%esp)
+	call   1630 <puts@plt+0xac0>
+	mov    %eax,0x4(%esp)
+	mov    %eax,%edi
+	mov    %ebp,(%esp)
+	movl   $0x0,0x28(%esp)
+	call   950 <printf@plt>
+	mov    %edi,0xc(%esp)
+	lea    -0x21da(%ebx),%eax
+	mov    %ebp,0x8(%esp)
+	movl   $0x3,(%esp)
+	mov    %eax,0x4(%esp)
+	call   960 <__android_log_print@plt>
+	movl   $0x4,0xc(%esp)
+	lea    0x28(%esp),%eax
+	mov    %edi,0x4(%esp)
+	mov    %esi,(%esp)
+	mov    %eax,0x8(%esp)
+	call   1210 <puts@plt+0x6a0>
+	mov    0x28(%esp),%eax
+	lea    0x7c(%esp),%esp
+	pop    %ebx
+	pop    %esi
+	pop    %edi
+	pop    %ebp
+	ret
+	lea    0x0(%esi,%eiz,1),%esi
+	push   %ebp
+	push   %edi
+	push   %esi
+	push   %ebx
+	call   114b <puts@plt+0x5db>
+	add    $0x2bfb,%ebx
+	lea    -0x2c(%esp),%esp
+	mov    0x4c(%esp),%eax
+	mov    0x48(%esp),%esi
+	mov    0x50(%esp),%edi
+	mov    %eax,0x8(%esp)
+	mov    0x40(%esp),%eax
+	mov    %esi,0x4(%esp)
+	mov    %edi,0xc(%esp)
+	mov    %eax,(%esp)
+	call   1210 <puts@plt+0x6a0>
+	test   %eax,%eax
+	js     2440 <puts@plt+0x18d0>
+	mov    %edi,%ebp
+	sub    $0x1,%ebp
+	js     2438 <puts@plt+0x18c8>
+	mov    0x4c(%esp),%eax
+	mov    0x44(%esp),%edx
+	movzbl -0x1(%eax,%edi,1),%eax
+	cmp    %al,-0x1(%edx,%edi,1)
+	je     2418 <puts@plt+0x18a8>
+	mov    %ebp,0x8(%esp)
+	lea    -0x1d68(%ebx),%edi
+	mov    %esi,0x4(%esp)
+	mov    %edi,(%esp)
+	call   950 <printf@plt>
+	mov    %edi,0x8(%esp)
+	lea    -0x21da(%ebx),%eax
+	mov    %ebp,0x10(%esp)
+	lea    0x1(%ebp),%edi
 	mov    %esi,0xc(%esp)
-	movl   $0x4,(%esp)
+	movl   $0x3,(%esp)
 	mov    %eax,0x4(%esp)
-	call   900 <__android_log_print@plt>
+	call   960 <__android_log_print@plt>
+	mov    0x44(%esp),%eax
+	mov    %edi,0xc(%esp)
+	mov    %esi,0x4(%esp)
+	mov    %eax,0x8(%esp)
+	mov    0x40(%esp),%eax
+	mov    %eax,(%esp)
+	call   12f0 <puts@plt+0x780>
+	test   %eax,%eax
+	js     2440 <puts@plt+0x18d0>
+	lea    0x2c(%esp),%esp
+	mov    %edi,%eax
+	pop    %ebx
+	pop    %esi
+	pop    %edi
+	pop    %ebp
+	ret
+	nop
+	lea    0x0(%esi,%eiz,1),%esi
+	sub    $0x1,%ebp
+	cmp    $0xffffffff,%ebp
+	je     2438 <puts@plt+0x18c8>
+	mov    0x4c(%esp),%eax
+	mov    0x44(%esp),%ecx
+	movzbl (%eax,%ebp,1),%eax
+	cmp    %al,(%ecx,%ebp,1)
+	jne    23ad <puts@plt+0x183d>
+	jmp    2418 <puts@plt+0x18a8>
+	nop
+	xor    %edi,%edi
+	jmp    2408 <puts@plt+0x1898>
+	lea    0x0(%esi,%eiz,1),%esi
+	mov    $0xffffffff,%edi
+	jmp    2408 <puts@plt+0x1898>
+	mov    %esi,%esi
+	lea    0x0(%edi,%eiz,1),%edi
+	push   %ebp
+	mov    $0x40,%ecx
+	push   %edi
+	push   %esi
+	push   %ebx
+	call   114b <puts@plt+0x5db>
+	add    $0x2af6,%ebx
+	lea    -0x13c(%esp),%esp
+	mov    0x15c(%esp),%eax
+	lea    0x2c(%esp),%edi
+	mov    0x158(%esp),%esi
+	mov    0x164(%esp),%ebp
+	mov    %eax,0x18(%esp)
+	mov    -0x10(%ebx),%eax
+	mov    (%eax),%eax
+	mov    %eax,0x12c(%esp)
+	xor    %eax,%eax
+	rep stos %eax,%es:(%edi)
+	mov    0x154(%esp),%eax
+	lea    0x2c(%esp),%edi
+	movl   $0x10,0x10(%esp)
+	mov    %esi,0x8(%esp)
+	mov    %eax,0x4(%esp)
+	mov    0x150(%esp),%eax
+	mov    %edi,0xc(%esp)
+	mov    %eax,(%esp)
+	call   2350 <puts@plt+0x17e0>
+	test   %eax,%eax
+	js     2550 <puts@plt+0x19e0>
+	mov    %eax,0x1c(%esp)
+	mov    0x160(%esp),%eax
+	mov    %ebp,0x10(%esp)
+	mov    %esi,0x4(%esp)
+	mov    %eax,0xc(%esp)
+	mov    0x18(%esp),%eax
+	mov    %eax,0x8(%esp)
+	mov    0x150(%esp),%eax
+	mov    %eax,(%esp)
+	call   1630 <puts@plt+0xac0>
 	mov    0x1c(%esp),%edx
+	mov    %eax,%ebp
 	test   %edx,%edx
-	je     1a00 <get_jni_env+0xf0>
-	add    %edx,%ebp
-	call   *%ebp
-	lea    0x2c(%esp),%esp
+	je     252e <puts@plt+0x19be>
+	mov    0x150(%esp),%eax
+	mov    %edx,0xc(%esp)
+	mov    %edi,0x8(%esp)
+	mov    %esi,0x4(%esp)
+	mov    %eax,(%esp)
+	call   12f0 <puts@plt+0x780>
+	test   %eax,%eax
+	mov    $0xffffffff,%eax
+	cmovs  %eax,%ebp
+	mov    -0x10(%ebx),%esi
+	mov    %ebp,%eax
+	mov    0x12c(%esp),%ecx
+	mov    (%esi),%edx
+	cmp    %edx,%ecx
+	jne    2578 <puts@plt+0x1a08>
+	lea    0x13c(%esp),%esp
 	pop    %ebx
 	pop    %esi
 	pop    %edi
 	pop    %ebp
 	ret
 	nop
+	mov    %eax,0x8(%esp)
+	lea    -0x2046(%ebx),%eax
+	mov    %eax,0x4(%esp)
+	mov    $0xffffffff,%ebp
+	mov    -0xc(%ebx),%eax
+	add    $0xa8,%eax
+	mov    %eax,(%esp)
+	call   ab0 <fprintf@plt>
+	jmp    252e <puts@plt+0x19be>
+	call   1130 <puts@plt+0x5c0>
+	lea    0x0(%esi),%esi
+	push   %ebp
+	push   %edi
+	push   %esi
+	push   %ebx
+	call   114b <puts@plt+0x5db>
+	add    $0x29cb,%ebx
+	lea    -0xec(%esp),%esp
+	lea    -0x2034(%ebx),%esi
+	mov    0x100(%esp),%ebp
+	mov    %esi,(%esp)
+	mov    %ebp,0x4(%esp)
+	call   950 <printf@plt>
+	mov    %esi,0x8(%esp)
+	lea    -0x21da(%ebx),%eax
+	mov    %ebp,0xc(%esp)
+	movl   $0x3,(%esp)
+	mov    %eax,0x4(%esp)
+	mov    %eax,0x18(%esp)
+	call   960 <__android_log_print@plt>
+	mov    0x114(%esp),%eax
+	mov    %ebp,(%esp)
+	mov    %eax,0x4(%esp)
+	call   17e0 <puts@plt+0xc70>
+	cmp    $0xffffffff,%eax
+	mov    %eax,%esi
+	je     2816 <puts@plt+0x1ca6>
+	mov    %ebp,(%esp)
+	lea    0x58(%esp),%eax
+	mov    %eax,0x4(%esp)
+	mov    %eax,0x1c(%esp)
+	call   14b0 <puts@plt+0x940>
+	cmp    $0xffffffff,%eax
+	mov    %eax,%esi
+	je     280e <puts@plt+0x1c9e>
+	mov    0x1c(%esp),%esi
+	lea    0x9c(%esp),%edi
+	mov    %edi,0x20(%esp)
+	mov    $0x11,%ecx
+	rep movsl %ds:(%esi),%es:(%edi)
+	call   1150 <puts@plt+0x5e0>
+	mov    0x1c(%esp),%esi
+	mov    %eax,%edi
+	movl   $0x1000,0x4(%esp)
+	mov    %ebp,(%esp)
+	mov    %esi,0x8(%esp)
+	call   2090 <puts@plt+0x1520>
+	cmp    $0xffffffff,%eax
+	mov    %eax,%esi
+	je     2b88 <puts@plt+0x2018>
+	cmp    $0x19,%edi
+	jg     2a20 <puts@plt+0x1eb0>
+	mov    -0x8(%ebx),%eax
+	mov    %ebp,(%esp)
+	mov    %eax,0x8(%esp)
+	lea    0x22c(%ebx),%eax
+	mov    %eax,0x4(%esp)
+	call   1b40 <puts@plt+0xfd0>
+	mov    %eax,%edi
+	lea    0x12c(%ebx),%edx
+	mov    %edx,(%esp)
+	lea    -0x1f77(%ebx),%eax
+	mov    %eax,0x4(%esp)
+	mov    %edx,0x24(%esp)
+	call   1e50 <puts@plt+0x12e0>
+	mov    0x24(%esp),%edx
+	mov    %eax,0x8(%esp)
+	mov    %ebp,(%esp)
+	mov    %edx,0x4(%esp)
+	call   1b40 <puts@plt+0xfd0>
+	mov    %eax,0x8(%esp)
+	lea    -0x1c30(%ebx),%edx
+	mov    %edi,0x4(%esp)
+	mov    %edx,(%esp)
+	mov    %eax,0x28(%esp)
+	mov    %edx,0x24(%esp)
+	call   950 <printf@plt>
+	mov    0x24(%esp),%edx
+	mov    0x28(%esp),%ecx
+	mov    0x18(%esp),%eax
+	mov    %edi,0xc(%esp)
+	mov    %edx,0x8(%esp)
+	mov    %ecx,0x10(%esp)
+	movl   $0x3,(%esp)
+	mov    %eax,0x4(%esp)
+	call   960 <__android_log_print@plt>
+	mov    0x104(%esp),%ecx
+	mov    %esi,0x4(%esp)
+	mov    %ebp,(%esp)
+	mov    %ecx,0x8(%esp)
+	call   1410 <puts@plt+0x8a0>
+	mov    0x104(%esp),%ecx
+	lea    -0x1d18(%ebx),%edx
+	mov    %edx,(%esp)
+	mov    %esi,0x30(%esp)
+	mov    %ecx,0x4(%esp)
+	movl   $0x2,0x34(%esp)
+	mov    %edx,0x24(%esp)
+	call   950 <printf@plt>
+	mov    0x104(%esp),%ecx
+	mov    0x24(%esp),%edx
+	mov    0x18(%esp),%eax
+	movl   $0x3,(%esp)
+	mov    %ecx,0xc(%esp)
+	mov    %edx,0x8(%esp)
+	mov    %eax,0x4(%esp)
+	call   960 <__android_log_print@plt>
+	mov    -0x8(%ebx),%ecx
+	mov    $0x2,%eax
+	mov    0x1c(%esp),%edx
+	mov    %eax,0x10(%esp)
+	lea    0x30(%esp),%eax
+	mov    %ecx,0x4(%esp)
+	mov    %edi,0x8(%esp)
+	mov    %edx,0x14(%esp)
+	mov    %ebp,(%esp)
+	mov    %eax,0xc(%esp)
+	mov    %eax,0x24(%esp)
+	call   2450 <puts@plt+0x18e0>
+	lea    -0x1cec(%ebx),%edx
+	mov    %eax,%edi
+	mov    %eax,0x4(%esp)
+	mov    %edx,(%esp)
+	mov    %edx,0x28(%esp)
+	call   950 <printf@plt>
+	mov    0x28(%esp),%edx
+	mov    0x18(%esp),%eax
+	mov    %edi,0xc(%esp)
+	sub    $0x1,%edi
+	movl   $0x3,(%esp)
+	mov    %edx,0x8(%esp)
+	mov    %eax,0x4(%esp)
+	call   960 <__android_log_print@plt>
+	cmp    $0xfffffffd,%edi
+	jbe    2828 <puts@plt+0x1cb8>
+	mov    %ebp,(%esp)
+	call   2260 <puts@plt+0x16f0>
+	mov    %eax,0xc(%esp)
+	mov    0x104(%esp),%eax
+	mov    %eax,0x8(%esp)
+	lea    -0x1fc1(%ebx),%eax
+	mov    %eax,0x4(%esp)
+	mov    $0xffffffff,%esi
+	mov    -0xc(%ebx),%eax
+	add    $0xa8,%eax
+	mov    %eax,(%esp)
+	call   ab0 <fprintf@plt>
+	mov    0x20(%esp),%eax
+	mov    %ebp,(%esp)
+	mov    %eax,0x4(%esp)
+	call   1510 <puts@plt+0x9a0>
+	mov    %ebp,(%esp)
+	call   1780 <puts@plt+0xc10>
+	lea    0xec(%esp),%esp
+	mov    %esi,%eax
+	pop    %ebx
+	pop    %esi
+	pop    %edi
+	pop    %ebp
+	ret
 	lea    0x0(%esi,%eiz,1),%esi
-	mov    %edi,0x10(%esp)
-	lea    -0x230d(%ebx),%eax
+	mov    0x108(%esp),%eax
+	mov    %eax,0x4(%esp)
+	mov    0x104(%esp),%eax
+	mov    %eax,(%esp)
+	call   1b80 <puts@plt+0x1010>
+	mov    %eax,%edi
+	mov    0x104(%esp),%eax
+	test   %edi,%edi
+	je     2b68 <puts@plt+0x1ff8>
+	mov    %eax,0x4(%esp)
+	mov    %ebp,(%esp)
+	call   19f0 <puts@plt+0xe80>
+	mov    %eax,0x8(%esp)
+	lea    -0x1ccc(%ebx),%ecx
+	mov    %eax,0x28(%esp)
+	mov    0x104(%esp),%eax
+	mov    %ecx,(%esp)
+	mov    %ecx,0x2c(%esp)
+	mov    %eax,0x4(%esp)
+	call   950 <printf@plt>
+	mov    0x104(%esp),%eax
+	mov    0x28(%esp),%edx
+	mov    0x2c(%esp),%ecx
+	mov    %eax,0xc(%esp)
+	mov    0x18(%esp),%eax
+	mov    %edx,0x10(%esp)
+	movl   $0x3,(%esp)
+	mov    %ecx,0x8(%esp)
+	mov    %eax,0x4(%esp)
+	call   960 <__android_log_print@plt>
+	mov    0x28(%esp),%edx
+	test   %edx,%edx
+	je     2bc0 <puts@plt+0x2050>
+	mov    0x108(%esp),%ecx
+	lea    (%edx,%edi,1),%eax
 	mov    %eax,0x8(%esp)
+	lea    -0x1cac(%ebx),%edi
+	mov    %edi,(%esp)
+	mov    %ecx,0x4(%esp)
+	mov    %eax,0x28(%esp)
+	call   950 <printf@plt>
+	mov    0x28(%esp),%eax
+	mov    %edi,0x8(%esp)
+	xor    %edi,%edi
+	movl   $0x3,(%esp)
+	mov    %eax,0x10(%esp)
+	mov    0x108(%esp),%eax
+	mov    %eax,0xc(%esp)
 	mov    0x18(%esp),%eax
-	mov    %esi,0xc(%esp)
-	movl   $0x6,(%esp)
 	mov    %eax,0x4(%esp)
-	call   900 <__android_log_print@plt>
+	call   960 <__android_log_print@plt>
+	mov    0x110(%esp),%edx
 	xor    %eax,%eax
-	jmp    1965 <get_jni_env+0x55>
-	movl   $0x6,(%esp)
-	lea    -0x21c4(%ebx),%eax
+	test   %edx,%edx
+	je     2980 <puts@plt+0x1e10>
+	mov    %ebp,0x100(%esp)
+	lea    0x0(%esi),%esi
+	lea    0x0(%edi),%edi
+	mov    0x10c(%esp),%ecx
+	lea    (%ecx,%eax,4),%ebp
+	mov    0x0(%ebp),%eax
+	mov    %esi,0x4(%esp)
 	mov    %eax,0x8(%esp)
+	mov    0x100(%esp),%eax
+	mov    %eax,(%esp)
+	call   1410 <puts@plt+0x8a0>
+	mov    0x24(%esp),%eax
+	mov    %esi,(%eax,%edi,4)
+	add    $0x1,%edi
+	mov    0x0(%ebp),%eax
+	mov    %eax,(%esp)
+	call   990 <strlen@plt>
+	add    %eax,%esi
+	mov    %edi,%eax
+	add    $0x1,%esi
+	cmp    0x110(%esp),%edi
+	jne    2930 <puts@plt+0x1dc0>
+	mov    0x100(%esp),%ebp
+	mov    0x108(%esp),%eax
+	lea    -0x1c88(%ebx),%esi
+	mov    %esi,(%esp)
+	lea    -0x1c5c(%ebx),%edi
+	mov    %eax,0x4(%esp)
+	call   950 <printf@plt>
+	mov    0x108(%esp),%eax
+	mov    %esi,0x8(%esp)
+	movl   $0x3,(%esp)
+	mov    %eax,0xc(%esp)
 	mov    0x18(%esp),%eax
 	mov    %eax,0x4(%esp)
-	call   900 <__android_log_print@plt>
-	xor    %eax,%eax
-	jmp    1965 <get_jni_env+0x55>
+	call   960 <__android_log_print@plt>
+	mov    0x1c(%esp),%ecx
+	mov    %ebp,(%esp)
+	mov    %ecx,0x10(%esp)
+	mov    0x110(%esp),%ecx
+	mov    %ecx,0xc(%esp)
+	mov    0x24(%esp),%ecx
+	mov    %ecx,0x8(%esp)
+	mov    0x28(%esp),%ecx
+	mov    %ecx,0x4(%esp)
+	call   1630 <puts@plt+0xac0>
+	mov    %eax,0x4(%esp)
+	mov    %eax,%esi
+	mov    %edi,(%esp)
+	call   950 <printf@plt>
+	mov    0x18(%esp),%eax
+	mov    %esi,0xc(%esp)
+	mov    %edi,0x8(%esp)
+	movl   $0x3,(%esp)
+	mov    %eax,0x4(%esp)
+	call   960 <__android_log_print@plt>
+	jmp    27fe <puts@plt+0x1c8e>
+	lea    0x0(%esi,%eiz,1),%esi
+	lea    -0x2019(%ebx),%eax
+	lea    0x22c(%ebx),%edi
+	mov    %eax,0x4(%esp)
+	mov    %edi,(%esp)
+	call   1e50 <puts@plt+0x12e0>
+	test   %eax,%eax
+	mov    %eax,%ecx
+	je     2bf2 <puts@plt+0x2082>
+	mov    %ecx,0x8(%esp)
+	mov    %edi,0x4(%esp)
+	mov    %ebp,(%esp)
+	mov    %ecx,0x2c(%esp)
+	call   1b40 <puts@plt+0xfd0>
+	mov    %eax,%edi
+	lea    0x12c(%ebx),%edx
+	mov    %edx,(%esp)
+	lea    -0x1f77(%ebx),%eax
+	mov    %eax,0x4(%esp)
+	mov    %edx,0x24(%esp)
+	call   1e50 <puts@plt+0x12e0>
+	mov    0x24(%esp),%edx
+	mov    %eax,0x8(%esp)
+	mov    %ebp,(%esp)
+	mov    %edx,0x4(%esp)
+	call   1b40 <puts@plt+0xfd0>
+	mov    %eax,0x8(%esp)
+	lea    -0x1c30(%ebx),%edx
+	mov    %edi,0x4(%esp)
+	mov    %edx,(%esp)
+	mov    %eax,0x24(%esp)
+	mov    %edx,0x28(%esp)
+	call   950 <printf@plt>
+	mov    0x24(%esp),%eax
+	mov    0x28(%esp),%edx
+	mov    %edi,0xc(%esp)
+	mov    %eax,0x10(%esp)
+	mov    0x18(%esp),%eax
+	movl   $0x3,(%esp)
+	mov    %edx,0x8(%esp)
+	mov    %eax,0x4(%esp)
+	call   960 <__android_log_print@plt>
+	mov    0x104(%esp),%eax
+	mov    %esi,0x4(%esp)
+	mov    %ebp,(%esp)
+	mov    %eax,0x8(%esp)
+	call   1410 <puts@plt+0x8a0>
+	mov    0x2c(%esp),%ecx
+	lea    0x32c(%ebx),%eax
+	mov    %ebp,(%esp)
+	mov    %eax,0x4(%esp)
+	mov    %esi,0x30(%esp)
+	movl   $0x2,0x34(%esp)
+	mov    %ecx,0x28(%esp)
+	call   19f0 <puts@plt+0xe80>
+	mov    %eax,0x38(%esp)
+	lea    -0x1d18(%ebx),%edx
+	mov    0x104(%esp),%eax
+	mov    %edx,(%esp)
+	mov    %edx,0x24(%esp)
+	mov    %eax,0x4(%esp)
+	call   950 <printf@plt>
+	mov    0x104(%esp),%eax
+	mov    0x24(%esp),%edx
+	movl   $0x3,(%esp)
+	mov    %eax,0xc(%esp)
+	mov    0x18(%esp),%eax
+	mov    %edx,0x8(%esp)
+	mov    %eax,0x4(%esp)
+	call   960 <__android_log_print@plt>
+	mov    0x28(%esp),%ecx
+	mov    $0x3,%eax
+	jmp    275d <puts@plt+0x1bed>
+	lea    0x0(%esi,%eiz,1),%esi
+	mov    %eax,0xc(%esp)
+	mov    0x108(%esp),%eax
+	mov    %eax,0x8(%esp)
+	lea    -0x1fac(%ebx),%eax
+	jmp    27e2 <puts@plt+0x1c72>
+	lea    0x0(%esi),%esi
+	mov    -0xc(%ebx),%eax
+	movl   $0x26,0x8(%esp)
+	movl   $0x1,0x4(%esp)
+	add    $0xa8,%eax
+	mov    %eax,0xc(%esp)
+	lea    -0x1d40(%ebx),%eax
+	mov    %eax,(%esp)
+	call   b20 <fwrite@plt>
+	jmp    27fe <puts@plt+0x1c8e>
+	lea    0x0(%esi),%esi
+	mov    0x104(%esp),%eax
+	mov    $0xffffffff,%esi
+	mov    %eax,0x8(%esp)
+	lea    -0x1f8e(%ebx),%eax
+	mov    %eax,0x4(%esp)
+	mov    -0xc(%ebx),%eax
+	add    $0xa8,%eax
+	mov    %eax,(%esp)
+	call   ab0 <fprintf@plt>
+	jmp    27fe <puts@plt+0x1c8e>
+	mov    %edi,(%esp)
+	lea    -0x2004(%ebx),%eax
+	mov    %eax,0x4(%esp)
+	call   1e50 <puts@plt+0x12e0>
+	test   %eax,%eax
+	mov    %eax,%ecx
+	jne    2a42 <puts@plt+0x1ed2>
+	mov    %edi,(%esp)
+	lea    -0x1fec(%ebx),%eax
+	mov    %eax,0x4(%esp)
+	call   1e50 <puts@plt+0x12e0>
+	test   %eax,%eax
+	mov    %eax,%ecx
+	jne    2a42 <puts@plt+0x1ed2>
+	mov    -0xc(%ebx),%eax
+	mov    $0xffffffff,%esi
+	movl   $0x1a,0x8(%esp)
+	movl   $0x1,0x4(%esp)
+	add    $0xa8,%eax
+	mov    %eax,0xc(%esp)
+	lea    -0x1fdc(%ebx),%eax
+	mov    %eax,(%esp)
+	call   b20 <fwrite@plt>
+	jmp    27fe <puts@plt+0x1c8e>
+	jmp    2c70 <puts@plt+0x2100>
+	nop
+	nop
+	nop
+	nop
+	nop
+	nop
+	nop
+	nop
+	nop
+	nop
+	nop
+	nop
+	nop
+	push   %edi
+	push   %esi
+	push   %ebx
+	call   114b <puts@plt+0x5db>
+	add    $0x22dc,%ebx
+	lea    -0x10(%esp),%esp
+	mov    0x28(%esp),%eax
+	mov    0x24(%esp),%edi
+	lea    -0x1(%eax),%esi
+	mov    0x20(%esp),%eax
+	mov    %edi,0x4(%esp)
+	mov    %esi,0x8(%esp)
+	mov    %eax,(%esp)
+	call   b30 <readlink@plt>
+	test   %eax,%eax
+	js     2cb8 <puts@plt+0x2148>
+	cmp    %eax,%esi
+	jle    2cb8 <puts@plt+0x2148>
+	movb   $0x0,(%edi,%eax,1)
+	lea    0x10(%esp),%esp
+	pop    %ebx
+	pop    %esi
+	pop    %edi
+	ret
+	lea    0x0(%esi),%esi
+	lea    -0x1f6f(%ebx),%eax
+	mov    %eax,(%esp)
+	call   9a0 <perror@plt>
+	lea    0x10(%esp),%esp
+	pop    %ebx
+	pop    %esi
+	pop    %edi
+	ret
+	xchg   %ax,%ax
+	push   %esi
+	push   %ebx
+	call   114b <puts@plt+0x5db>
+	add    $0x227d,%ebx
+	lea    -0x74(%esp),%esp
+	mov    0x80(%esp),%esi
+	lea    0x10(%esp),%eax
+	mov    %eax,0x4(%esp)
+	mov    %esi,(%esp)
+	call   b40 <lstat@plt>
+	mov    0x20(%esp),%eax
+	and    $0xf000,%eax
+	cmp    $0xa000,%eax
+	je     2d10 <puts@plt+0x21a0>
+	lea    0x74(%esp),%esp
+	pop    %ebx
+	pop    %esi
+	ret
+	nop
+	mov    %esi,0x4(%esp)
+	mov    %esi,(%esp)
+	movl   $0x100,0x8(%esp)
+	call   2c70 <puts@plt+0x2100>
+	lea    0x74(%esp),%esp
+	pop    %ebx
+	pop    %esi
+	ret
+	nop
+	lea    0x0(%esi,%eiz,1),%esi
```

#### .rodata

```diff
@@ -1,835 +1,1157 @@
 00000000: 7f45 4c46 0101 0100 0000 0000 0000 0000  .ELF............
-00000010: 0300 0300 0100 0000 0000 0000 3400 0000  ............4...
-00000020: e430 0000 0000 0000 3400 2000 0700 2800  .0......4. ...(.
-00000030: 1500 1400 0600 0000 3400 0000 3400 0000  ........4...4...
-00000040: 3400 0000 e000 0000 e000 0000 0400 0000  4...............
-00000050: 0400 0000 0100 0000 0000 0000 0000 0000  ................
-00000060: 0000 0000 9021 0000 9021 0000 0500 0000  .....!...!......
-00000070: 0010 0000 0100 0000 5c2e 0000 5c3e 0000  ........\...\>..
-00000080: 5c3e 0000 a801 0000 a801 0000 0600 0000  \>..............
-00000090: 0010 0000 0200 0000 682e 0000 683e 0000  ........h...h>..
-000000a0: 683e 0000 0001 0000 0001 0000 0600 0000  h>..............
-000000b0: 0400 0000 50e5 7464 0c21 0000 0c21 0000  ....P.td.!...!..
-000000c0: 0c21 0000 8400 0000 8400 0000 0400 0000  .!..............
-000000d0: 0400 0000 51e5 7464 0000 0000 0000 0000  ....Q.td........
-000000e0: 0000 0000 0000 0000 0000 0000 0600 0000  ................
-000000f0: 0000 0000 52e5 7464 5c2e 0000 5c3e 0000  ....R.td\...\>..
-00000100: 5c3e 0000 a401 0000 a401 0000 0600 0000  \>..............
-00000110: 0400 0000 0000 0000 0000 0000 0000 0000  ................
-00000120: 0000 0000 0100 0000 0000 0000 0000 0000  ................
-00000130: 1200 0000 1000 0000 0000 0000 0000 0000  ................
-00000140: 1200 0000 1d00 0000 0000 0000 0000 0000  ................
-00000150: 1200 0000 2e00 0000 a00b 0000 5503 0000  ............U...
-00000160: 1200 0700 4100 0000 0000 0000 0000 0000  ....A...........
-00000170: 1200 0000 5500 0000 0000 0000 0000 0000  ....U...........
-00000180: 1200 0000 5a00 0000 000f 0000 de03 0000  ....Z...........
-00000190: 1200 0700 6300 0000 0000 0000 0000 0000  ....c...........
-000001a0: 1100 0000 7500 0000 0000 0000 0000 0000  ....u...........
-000001b0: 1200 0000 7d00 0000 0000 0000 0000 0000  ....}...........
-000001c0: 1200 0000 8400 0000 0000 0000 0000 0000  ................
-000001d0: 1200 0000 8c00 0000 0000 0000 0000 0000  ................
-000001e0: 1200 0000 9300 0000 3013 0000 3d00 0000  ........0...=...
-000001f0: 1200 0700 a100 0000 1019 0000 4201 0000  ............B...
-00000200: 1200 0700 ad00 0000 0000 0000 0000 0000  ................
-00000210: 1200 0000 b400 0000 0000 0000 0000 0000  ................
-00000220: 1200 0000 c300 0000 0000 0000 0000 0000  ................
-00000230: 1200 0000 c900 0000 7013 0000 e300 0000  ........p.......
-00000240: 1200 0700 d200 0000 0000 0000 0000 0000  ................
-00000250: 1200 0000 d800 0000 e012 0000 1b00 0000  ................
-00000260: 1200 0700 0901 0000 0000 0000 0000 0000  ................
-00000270: 1200 0000 1001 0000 0013 0000 2500 0000  ............%...
-00000280: 1200 0700 4001 0000 0000 0000 0000 0000  ....@...........
-00000290: 1200 0000 4601 0000 0000 0000 0000 0000  ....F...........
-000002a0: 1200 0000 4b01 0000 0000 0000 0000 0000  ....K...........
-000002b0: 1200 0000 5101 0000 0000 0000 0000 0000  ....Q...........
-000002c0: 1200 0000 5701 0000 0000 0000 0000 0000  ....W...........
-000002d0: 1200 0000 5c01 0000 0000 0000 0000 0000  ....\...........
-000002e0: 1200 0000 6301 0000 6014 0000 f500 0000  ....c...`.......
-000002f0: 1200 0700 7301 0000 0000 0000 0000 0000  ....s...........
-00000300: 1200 0000 7a01 0000 0000 0000 0000 0000  ....z...........
-00000310: 1200 0000 8001 0000 0000 0000 0000 0000  ................
-00000320: 1200 0000 8701 0000 0000 0000 0000 0000  ................
-00000330: 1200 0000 8f01 0000 6015 0000 a603 0000  ........`.......
-00000340: 1200 0700 a101 0000 0000 0000 0000 0000  ................
-00000350: 1200 0000 a601 0000 0000 0000 0000 0000  ................
-00000360: 1200 0000 ac01 0000 0000 0000 0000 0000  ................
-00000370: 1200 0000 b101 0000 0000 0000 0000 0000  ................
-00000380: 1200 0000 b801 0000 0000 0000 0000 0000  ................
-00000390: 1200 0000 bd01 0000 0000 0000 0000 0000  ................
-000003a0: 1200 0000 c301 0000 0000 0000 0000 0000  ................
-000003b0: 1200 0000 ca01 0000 0000 0000 0000 0000  ................
-000003c0: 1200 0000 d101 0000 0000 0000 0000 0000  ................
-000003d0: 1200 0000 d701 0000 0440 0000 0000 0000  .........@......
-000003e0: 1000 f1ff de01 0000 0440 0000 0000 0000  .........@......
-000003f0: 1000 f1ff ea01 0000 0440 0000 0000 0000  .........@......
-00000400: 1000 f1ff 005f 5f63 7861 5f66 696e 616c  .....__cxa_final
-00000410: 697a 6500 5f5f 6378 615f 6174 6578 6974  ize.__cxa_atexit
-00000420: 005f 5f73 7461 636b 5f63 686b 5f66 6169  .__stack_chk_fai
-00000430: 6c00 6c6f 6164 5f64 6578 5f69 6e5f 7468  l.load_dex_in_th
-00000440: 7265 6164 005f 5f61 6e64 726f 6964 5f6c  read.__android_l
-00000450: 6f67 5f70 7269 6e74 0066 7265 6500 6c6f  og_print.free.lo
-00000460: 6164 5f64 6578 005f 5f73 7461 636b 5f63  ad_dex.__stack_c
-00000470: 686b 5f67 7561 7264 0073 7472 6e63 7079  hk_guard.strncpy
-00000480: 0067 6574 7569 6400 7370 7269 6e74 6600  .getuid.sprintf.
-00000490: 6163 6365 7373 0067 6574 5f66 696c 655f  access.get_file_
-000004a0: 7369 7a65 0067 6574 5f6a 6e69 5f65 6e76  size.get_jni_env
-000004b0: 006d 616c 6c6f 6300 7074 6872 6561 645f  .malloc.pthread_
-000004c0: 6372 6561 7465 0063 686d 6f64 0063 6f70  create.chmod.cop
-000004d0: 7966 696c 6500 6d6b 6469 7200 4a61 7661  yfile.mkdir.Java
-000004e0: 5f63 6f6d 5f74 6573 745f 616e 6472 6f69  _com_test_androi
-000004f0: 6473 7079 5f48 656c 7065 7255 7469 6c5f  dspy_HelperUtil_
-00000500: 6e61 7469 7665 5365 7473 6964 0073 6574  nativeSetsid.set
-00000510: 7369 6400 4a61 7661 5f63 6f6d 5f74 6573  sid.Java_com_tes
-00000520: 745f 616e 6472 6f69 6473 7079 5f48 656c  t_androidspy_Hel
-00000530: 7065 7255 7469 6c5f 6e61 7469 7665 556d  perUtil_nativeUm
-00000540: 6173 6b00 756d 6173 6b00 7374 6174 0066  ask.umask.stat.f
-00000550: 6f70 656e 0066 7075 7463 0067 6574 6300  open.fputc.getc.
-00000560: 6663 6c6f 7365 0067 6574 5f6d 6f64 756c  fclose.get_modul
-00000570: 655f 6261 7365 0073 7472 7374 7200 6667  e_base.strstr.fg
-00000580: 6574 7300 7374 7274 6f6b 0073 7472 746f  ets.strtok.strto
-00000590: 756c 0067 6574 5f73 796d 626f 6c5f 6f66  ul.get_symbol_of
-000005a0: 6673 6574 006f 7065 6e00 6673 7461 7400  fset.open.fstat.
-000005b0: 6d6d 6170 006d 656d 7365 7400 7265 6164  mmap.memset.read
-000005c0: 0063 6c6f 7365 0073 7472 636d 7000 6d75  .close.strcmp.mu
-000005d0: 6e6d 6170 0064 6c73 796d 005f 6564 6174  nmap.dlsym._edat
-000005e0: 6100 5f5f 6273 735f 7374 6172 7400 5f65  a.__bss_start._e
-000005f0: 6e64 006c 6962 6c6f 672e 736f 006c 6962  nd.liblog.so.lib
-00000600: 7374 6463 2b2b 2e73 6f00 6c69 626d 2e73  stdc++.so.libm.s
-00000610: 6f00 6c69 6263 2e73 6f00 6c69 6264 6c2e  o.libc.so.libdl.
-00000620: 736f 006c 6962 6465 786c 6f61 6465 722e  so.libdexloader.
-00000630: 736f 0000 2500 0000 2f00 0000 0000 0000  so..%.../.......
-00000640: 2900 0000 0000 0000 1300 0000 2a00 0000  )...........*...
-00000650: 2200 0000 2b00 0000 0700 0000 0000 0000  "...+...........
-00000660: 0000 0000 1f00 0000 2400 0000 0200 0000  ........$.......
-00000670: 0000 0000 2000 0000 1c00 0000 2800 0000  .... .......(...
-00000680: 2100 0000 2c00 0000 0b00 0000 0000 0000  !...,...........
-00000690: 2700 0000 0000 0000 0f00 0000 0e00 0000  '...............
-000006a0: 0000 0000 0000 0000 2500 0000 0d00 0000  ........%.......
-000006b0: 0000 0000 1e00 0000 2e00 0000 2600 0000  ............&...
-000006c0: 0000 0000 0000 0000 2d00 0000 0400 0000  ........-.......
-000006d0: 0000 0000 0000 0000 0000 0000 0100 0000  ................
-000006e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000006f0: 0000 0000 0000 0000 0500 0000 0000 0000  ................
-00000700: 0300 0000 0000 0000 0000 0000 0000 0000  ................
-00000710: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000720: 0000 0000 1400 0000 0600 0000 0c00 0000  ................
-00000730: 0000 0000 0000 0000 0000 0000 1100 0000  ................
-00000740: 0000 0000 1000 0000 1700 0000 0000 0000  ................
-00000750: 1900 0000 0000 0000 0000 0000 0a00 0000  ................
-00000760: 0800 0000 1200 0000 1a00 0000 2300 0000  ............#...
-00000770: 1500 0000 1b00 0000 0000 0000 1d00 0000  ................
-00000780: 1800 0000 0900 0000 1600 0000 5c3e 0000  ............\>..
-00000790: 0800 0000 6c3f 0000 0800 0000 0040 0000  ....l?.......@..
-000007a0: 0800 0000 683f 0000 0608 0000 7c3f 0000  ....h?......|?..
-000007b0: 0702 0000 803f 0000 0703 0000 843f 0000  .....?.......?..
-000007c0: 0701 0000 883f 0000 0705 0000 8c3f 0000  .....?.......?..
-000007d0: 0706 0000 903f 0000 0709 0000 943f 0000  .....?.......?..
-000007e0: 070a 0000 983f 0000 070b 0000 9c3f 0000  .....?.......?..
-000007f0: 070c 0000 a03f 0000 070f 0000 a43f 0000  .....?.......?..
-00000800: 0710 0000 a83f 0000 0711 0000 ac3f 0000  .....?.......?..
-00000810: 0713 0000 b03f 0000 0715 0000 b43f 0000  .....?.......?..
-00000820: 0717 0000 b83f 0000 0718 0000 bc3f 0000  .....?.......?..
-00000830: 0719 0000 c03f 0000 071a 0000 c43f 0000  .....?.......?..
-00000840: 071b 0000 c83f 0000 071c 0000 cc3f 0000  .....?.......?..
-00000850: 071e 0000 d03f 0000 071f 0000 d43f 0000  .....?.......?..
-00000860: 0720 0000 d83f 0000 0721 0000 dc3f 0000  . ...?...!...?..
-00000870: 0723 0000 e03f 0000 0724 0000 e43f 0000  .#...?...$...?..
-00000880: 0725 0000 e83f 0000 0726 0000 ec3f 0000  .%...?...&...?..
-00000890: 0727 0000 f03f 0000 0728 0000 f43f 0000  .'...?...(...?..
-000008a0: 0729 0000 f83f 0000 072a 0000 fc3f 0000  .)...?...*...?..
-000008b0: 072b 0000 0000 0000 0000 0000 0000 0000  .+..............
-000008c0: ffb3 0400 0000 ffa3 0800 0000 0000 0000  ................
-000008d0: ffa3 0c00 0000 6800 0000 00e9 e0ff ffff  ......h.........
-000008e0: ffa3 1000 0000 6808 0000 00e9 d0ff ffff  ......h.........
-000008f0: ffa3 1400 0000 6810 0000 00e9 c0ff ffff  ......h.........
-00000900: ffa3 1800 0000 6818 0000 00e9 b0ff ffff  ......h.........
-00000910: ffa3 1c00 0000 6820 0000 00e9 a0ff ffff  ......h ........
-00000920: ffa3 2000 0000 6828 0000 00e9 90ff ffff  .. ...h(........
-00000930: ffa3 2400 0000 6830 0000 00e9 80ff ffff  ..$...h0........
-00000940: ffa3 2800 0000 6838 0000 00e9 70ff ffff  ..(...h8....p...
-00000950: ffa3 2c00 0000 6840 0000 00e9 60ff ffff  ..,...h@....`...
-00000960: ffa3 3000 0000 6848 0000 00e9 50ff ffff  ..0...hH....P...
-00000970: ffa3 3400 0000 6850 0000 00e9 40ff ffff  ..4...hP....@...
-00000980: ffa3 3800 0000 6858 0000 00e9 30ff ffff  ..8...hX....0...
-00000990: ffa3 3c00 0000 6860 0000 00e9 20ff ffff  ..<...h`.... ...
-000009a0: ffa3 4000 0000 6868 0000 00e9 10ff ffff  ..@...hh........
-000009b0: ffa3 4400 0000 6870 0000 00e9 00ff ffff  ..D...hp........
-000009c0: ffa3 4800 0000 6878 0000 00e9 f0fe ffff  ..H...hx........
-000009d0: ffa3 4c00 0000 6880 0000 00e9 e0fe ffff  ..L...h.........
-000009e0: ffa3 5000 0000 6888 0000 00e9 d0fe ffff  ..P...h.........
-000009f0: ffa3 5400 0000 6890 0000 00e9 c0fe ffff  ..T...h.........
-00000a00: ffa3 5800 0000 6898 0000 00e9 b0fe ffff  ..X...h.........
-00000a10: ffa3 5c00 0000 68a0 0000 00e9 a0fe ffff  ..\...h.........
-00000a20: ffa3 6000 0000 68a8 0000 00e9 90fe ffff  ..`...h.........
-00000a30: ffa3 6400 0000 68b0 0000 00e9 80fe ffff  ..d...h.........
-00000a40: ffa3 6800 0000 68b8 0000 00e9 70fe ffff  ..h...h.....p...
-00000a50: ffa3 6c00 0000 68c0 0000 00e9 60fe ffff  ..l...h.....`...
-00000a60: ffa3 7000 0000 68c8 0000 00e9 50fe ffff  ..p...h.....P...
-00000a70: ffa3 7400 0000 68d0 0000 00e9 40fe ffff  ..t...h.....@...
-00000a80: ffa3 7800 0000 68d8 0000 00e9 30fe ffff  ..x...h.....0...
-00000a90: ffa3 7c00 0000 68e0 0000 00e9 20fe ffff  ..|...h..... ...
-00000aa0: ffa3 8000 0000 68e8 0000 00e9 10fe ffff  ......h.........
-00000ab0: ffa3 8400 0000 68f0 0000 00e9 00fe ffff  ......h.........
-00000ac0: ffa3 8800 0000 68f8 0000 00e9 f0fd ffff  ......h.........
-00000ad0: ffa3 8c00 0000 6800 0100 00e9 e0fd ffff  ......h.........
-00000ae0: 53e8 aa00 0000 81c3 8a34 0000 8d64 24e8  S........4...d$.
-00000af0: 8d83 9000 0000 8904 24e8 f2fd ffff 8d64  ........$......d
-00000b00: 2418 5bc3 0000 0000 0000 0000 0000 0000  $.[.............
-00000b10: 8d64 24f4 8b44 2410 85c0 7402 ffd0 8d64  .d$..D$...t....d
-00000b20: 240c c38d b600 0000 008d bc27 0000 0000  $..........'....
-00000b30: 53e8 5a00 0000 81c3 3a34 0000 8d64 24e8  S.Z.....:4...d$.
-00000b40: 8d83 9000 0000 8944 2408 8b44 2420 8944  .......D$..D$ .D
-00000b50: 2404 8d83 a0cb ffff 8904 24e8 70fd ffff  $.........$.p...
-00000b60: 8d64 2418 5bc3 8d76 008d bc27 0000 0000  .d$.[..v...'....
-00000b70: 53e8 1a00 0000 81c3 fa33 0000 8d64 24f8  S........3...d$.
-00000b80: e85b fdff ff8d 6424 085b c390 8d74 2600  .[....d$.[...t&.
-00000b90: 8b1c 24c3 908d b426 0000 0000 0000 0000  ..$....&........
-00000ba0: 5557 5653 e8e7 ffff ff81 c3c7 3300 008d  UWVS........3...
-00000bb0: 6424 b48d 83e4 daff ff89 4424 088d abf1  d$........D$....
-00000bc0: daff ffc7 0424 0400 0000 896c 2404 e82d  .....$.....l$..-
-00000bd0: fdff ff8b 4424 608d 5424 3cc7 4424 3c00  ....D$`.T$<.D$<.
-00000be0: 0000 008b 0089 4424 2c89 c78b 00c7 4424  ......D$,.....D$
-00000bf0: 0800 0000 0089 5424 0489 3c24 ff50 108b  ......T$..<$.P..
-00000c00: 4424 3c85 c00f 84c5 0200 0089 4424 0c8d  D$<.........D$..
-00000c10: 830a dbff ff89 6c24 04c7 0424 0400 0000  ......l$...$....
-00000c20: 8944 2408 e8d7 fcff ff8b 4424 3c8d 8b1d  .D$.......D$<...
-00000c30: dbff ff8b 1089 4c24 0489 0424 ff52 188d  ......L$...$.R..
-00000c40: 8b33 dbff ff89 c68b 4424 3c8b 1089 4c24  .3......D$<...L$
-00000c50: 0c8d 8b4d dbff ff89 7424 0489 0424 894c  ...M....t$...$.L
-00000c60: 2408 ff92 c401 0000 8b54 243c 8b0a 8974  $........T$<...t
-00000c70: 2404 8914 2489 4424 08ff 91c8 0100 008b  $...$.D$........
-00000c80: 7424 6089 4424 248b 4424 3c8d 4e04 8b10  t$`.D$$.D$<.N...
-00000c90: 894c 2404 8904 24ff 929c 0200 008b 7c24  .L$...$.......|$
-00000ca0: 6089 4424 288b 4424 3c8d 8f08 0100 008b  `.D$(.D$<.......
-00000cb0: 1089 4c24 0489 0424 ff92 9c02 0000 8d8b  ..L$...$........
-00000cc0: 62db ffff 89c7 8b44 243c 8b10 894c 2404  b......D$<...L$.
-00000cd0: 8904 24ff 5218 8b54 243c 8d8b 10dd ffff  ..$.R..T$<......
-00000ce0: 89c6 8b02 894c 240c 8d8b 7fdb ffff 8974  .....L$........t
-00000cf0: 2404 8914 2489 4c24 08ff 9084 0000 008b  $...$.L$........
-00000d00: 4c24 3c8b 5424 248b 0989 7c24 1089 4424  L$<.T$$...|$..D$
-00000d10: 088b 7c24 288b 4424 3c89 5424 1889 7424  ..|$(.D$<.T$..t$
-00000d20: 04c7 4424 1400 0000 0089 7c24 0c89 0424  ..D$......|$...$
-00000d30: ff51 7089 6c24 04c7 0424 0400 0000 8944  .Qp.l$...$.....D
-00000d40: 240c 89c7 8d83 86db ffff 8944 2408 e8ad  $..........D$...
-00000d50: fbff ff8b 4424 3c8d 8b64 ddff ff8b 1089  ....D$<..d......
-00000d60: 4c24 0c8d 8b9c dbff ff89 7424 0489 0424  L$........t$...$
-00000d70: 894c 2408 ff92 8400 0000 8b74 2460 8944  .L$........t$`.D
-00000d80: 2424 8b44 243c 81c6 0c02 0000 8b10 8974  $$.D$<.........t
-00000d90: 2404 8904 24ff 929c 0200 008b 5424 3c8b  $...$.......T$<.
-00000da0: 0a89 4424 0c8b 4424 2489 1424 897c 2404  ..D$..D$$..$.|$.
-00000db0: 8944 2408 ff91 8800 0000 8974 240c 896c  .D$........t$..l
-00000dc0: 2404 8944 2410 89c7 c704 2404 0000 008d  $..D$.....$.....
-00000dd0: 83a6 dbff ff89 4424 08e8 22fb ffff 8b44  ......D$.."....D
-00000de0: 243c 8b10 8904 24ff 523c 85c0 8b44 243c  $<....$.R<...D$<
-00000df0: 8b10 743c 8904 24ff 5240 8b44 243c 8b10  ..t<..$.R@.D$<..
-00000e00: 8904 24ff 5244 8974 240c 8d83 b3db ffff  ..$.RD.t$.......
-00000e10: 896c 2404 c704 2406 0000 0089 4424 08e8  .l$...$.....D$..
-00000e20: dcfa ffff 8d64 244c 31c0 5b5e 5f5d c390  .....d$L1.[^_]..
-00000e30: 8b74 2460 897c 2404 8904 248d 8e14 0400  .t$`.|$...$.....
-00000e40: 0089 4c24 0c8d 8e10 0300 0089 4c24 08ff  ..L$........L$..
-00000e50: 92c4 0100 008b 4c24 6089 c68b 4424 3c81  ......L$`...D$<.
-00000e60: c118 0500 008b 1089 4c24 0489 0424 ff92  ........L$...$..
-00000e70: 9c02 0000 8b54 243c 8b0a 8914 2489 4424  .....T$<....$.D$
-00000e80: 0c89 7424 0889 7c24 04ff 9134 0200 008b  ..t$..|$...4....
-00000e90: 7424 2c8b 0689 3424 ff50 148b 4424 6089  t$,...4$.P..D$`.
-00000ea0: 0424 e869 faff ff89 6c24 048d 83c8 dbff  .$.i....l$......
-00000eb0: ffc7 0424 0400 0000 8944 2408 e83f faff  ...$.....D$..?..
-00000ec0: ff8d 6424 4c31 c05b 5e5f 5dc3 8d74 2600  ..d$L1.[^_]..t&.
-00000ed0: 896c 2404 8d83 fbda ffff c704 2406 0000  .l$.........$...
-00000ee0: 0089 4424 08e8 16fa ffff 8d64 244c 31c0  ..D$.......d$L1.
-00000ef0: 5b5e 5f5d c38d 7426 008d bc27 0000 0000  [^_]..t&...'....
-00000f00: 5557 5653 e887 fcff ff81 c367 3000 008d  UWVS.......g0...
-00000f10: a424 94fc ffff 8b84 2480 0300 0089 4424  .$......$.....D$
-00000f20: 2c89 c18b 8424 8403 0000 8944 2424 89c6  ,....$.....D$$..
-00000f30: 8b84 2488 0300 0089 4424 3089 c28b 8424  ..$.....D$0....$
-00000f40: 8c03 0000 8944 2434 89c7 8b84 2490 0300  .....D$4....$...
-00000f50: 0089 4424 388b 8424 9403 0000 8944 243c  ..D$8..$.....D$<
-00000f60: 89c5 8b83 f8ff ffff 8b00 896c 241c 8dab  ...........l$...
-00000f70: f1da ffff 897c 2418 8d7c 2450 8984 245c  .....|$..|$P..$\
-00000f80: 0300 008d 838c ddff ff89 5424 1489 7424  ..........T$..t$
-00000f90: 1089 4c24 0c89 6c24 04c7 0424 0400 0000  ..L$..l$...$....
-00000fa0: 8944 2408 e857 f9ff ff31 c0b9 4100 0000  .D$..W...1..A...
-00000fb0: f3ab 8974 2404 8d74 2450 c744 2408 0401  ...t$..t$P.D$...
-00000fc0: 0000 8934 24e8 56f9 ffff 89f0 8d74 2600  ...4$.V......t&.
-00000fd0: 8038 0074 1383 c001 75f6 b8ff ffff ff90  .8.t....u.......
-00000fe0: 8038 2f8d 5001 740a 83e8 0175 f3ba 0100  .8/.P.t....u....
-00000ff0: 0000 c600 008d bc24 5401 0000 b941 0000  .......$T....A..
-00001000: 0031 c0f3 ab89 5424 048d 9424 5401 0000  .1....T$...$T...
-00001010: c744 2408 0401 0000 8914 2489 5424 28e8  .D$.......$.T$(.
-00001020: fcf8 ffff e807 f9ff ff89 4424 0c8d 83d4  ..........D$....
-00001030: dbff ff89 7424 0889 3424 8944 2404 e8fd  ....t$..4$.D$...
-00001040: f8ff ff89 7424 0c8d 83da dbff ff89 6c24  ....t$........l$
-00001050: 04c7 0424 0400 0000 8944 2408 e89f f8ff  ...$.....D$.....
-00001060: ffc7 4424 0400 0000 0089 3424 e8df f8ff  ..D$......4$....
-00001070: ff8b 5424 2883 f8ff 0f84 1a02 0000 31c0  ..T$(.........1.
-00001080: 8dbc 2458 0200 00b9 4100 0000 f3ab 8d83  ..$X....A.......
-00001090: ebdb ffff 8dbc 2458 0200 0089 5424 0c89  ......$X....T$..
-000010a0: 7424 0889 4424 0489 3c24 e891 f8ff ff8b  t$..D$..<$......
-000010b0: 4424 2489 0424 e875 0200 0085 c00f 8585  D$$..$.u........
-000010c0: 0100 00e8 4808 0000 8944 240c 89c7 896c  ....H....D$....l
-000010d0: 2404 8d83 f1db ffff c704 2404 0000 0089  $.........$.....
-000010e0: 4424 08e8 18f8 ffff 8b07 8d54 2448 8954  D$.........T$H.T
-000010f0: 2404 893c 24ff 906c 0300 0085 c00f 85ae  $..<$..l........
-00001100: 0100 008b 4424 4889 6c24 04c7 0424 0400  ....D$H.l$...$..
-00001110: 0000 8944 240c 8d83 10dc ffff 8944 2408  ...D$........D$.
-00001120: e8db f7ff ffc7 0424 1c06 0000 e82f f8ff  .......$...../..
-00001130: ff89 c78b 4424 4889 078b 4424 2cc7 4424  ....D$H...D$,.D$
-00001140: 0804 0100 0089 4424 048d 4704 8904 24e8  ......D$..G...$.
-00001150: ccf7 ffff c744 2408 0401 0000 8d87 0801  .....D$.........
-00001160: 0000 8974 2404 8904 24e8 b2f7 ffff 8b44  ...t$...$......D
-00001170: 2430 c744 2408 0401 0000 8944 2404 8d87  $0.D$......D$...
-00001180: 0c02 0000 8904 24e8 94f7 ffff 8b44 2434  ......$......D$4
-00001190: c744 2408 0401 0000 8944 2404 8d87 1003  .D$......D$.....
-000011a0: 0000 8904 24e8 76f7 ffff 8b44 2438 c744  ....$.v....D$8.D
-000011b0: 2408 0401 0000 8944 2404 8d87 1404 0000  $......D$.......
-000011c0: 8904 24e8 58f7 ffff 8b44 243c c744 2408  ..$.X....D$<.D$.
-000011d0: 0401 0000 8944 2404 8d87 1805 0000 8904  .....D$.........
-000011e0: 24e8 3af7 ffff 896c 2404 8d83 1bdc ffff  $.:....l$.......
-000011f0: c704 2404 0000 0089 4424 08e8 00f7 ffff  ..$.....D$......
-00001200: 8b83 fcff ffff 897c 240c c744 2404 0000  .......|$..D$...
-00001210: 0000 8944 2408 8d44 244c 8904 24e8 4ef7  ...D$..D$L..$.N.
-00001220: ffff 31c0 8b93 f8ff ffff 8b8c 245c 0300  ..1.........$\..
-00001230: 008b 1239 d10f 859e 0000 008d a424 6c03  ...9.........$l.
-00001240: 0000 5b5e 5f5d c390 893c 2489 4424 28e8  ..[^_]...<$.D$(.
-00001250: dc00 0000 8b54 2428 39c2 0f84 63fe ffff  .....T$(9...c...
-00001260: c744 2404 ff01 0000 8934 24e8 10f7 ffff  .D$......4$.....
-00001270: 8b44 2424 897c 2404 8904 24e8 f000 0000  .D$$.|$...$.....
-00001280: c744 2404 ff01 0000 893c 24e8 f0f6 ffff  .D$......<$.....
-00001290: e92e feff ff8d 7600 c744 2404 ff01 0000  ......v..D$.....
-000012a0: 8934 24e8 e8f6 ffff 8b54 2428 e9cd fdff  .4$......T$(....
-000012b0: ff89 4424 0c8d 83fd dbff ff89 6c24 04c7  ..D$........l$..
-000012c0: 0424 0600 0000 8944 2408 e831 f6ff ffb8  .$.....D$..1....
-000012d0: ffff ffff e94b ffff ffe8 92f8 ffff 6690  .....K........f.
-000012e0: 53e8 aaf8 ffff 81c3 8a2c 0000 8d64 24f8  S........,...d$.
-000012f0: e8ab f6ff ff8d 6424 085b c390 8d74 2600  ......d$.[...t&.
-00001300: 53e8 8af8 ffff 81c3 6a2c 0000 8d64 24e8  S.......j,...d$.
-00001310: 0fb7 4424 2889 0424 e893 f6ff ff8d 6424  ..D$(..$......d$
-00001320: 1831 c05b c38d 7426 008d bc27 0000 0000  .1.[..t&...'....
-00001330: 53e8 5af8 ffff 81c3 3a2c 0000 8d64 2488  S.Z.....:,...d$.
-00001340: 8d44 2410 8944 2404 8b84 2480 0000 0089  .D$..D$...$.....
-00001350: 0424 e869 f6ff ff85 c0ba ffff ffff 8b44  .$.i...........D
-00001360: 243c 0f49 d08d 6424 785b 89d0 c38d 7600  $<.I..d$x[....v.
-00001370: 5557 5653 e817 f8ff ff81 c3f7 2b00 008d  UWVS........+...
-00001380: 6424 d48d abf1 daff ff8b 4424 448b 7c24  d$........D$D.|$
-00001390: 4089 6c24 0489 4424 108d 8331 dcff ff89  @.l$..D$...1....
-000013a0: 7c24 0cc7 0424 0400 0000 8944 2408 e84d  |$...$.....D$..M
-000013b0: f5ff ff89 3c24 8d83 40dc ffff 8944 2404  ....<$..@....D$.
-000013c0: e80b f6ff ff85 c089 c674 598d 8354 dcff  .........tY..T..
-000013d0: ff89 4424 048b 4424 4489 0424 e8ef f5ff  ..D$..D$D..$....
-000013e0: ff85 c089 c775 15eb 608d b426 0000 0000  .....u..`..&....
-000013f0: 897c 2404 8904 24e8 e4f5 ffff 8934 24e8  .|$...$......4$.
-00001400: ecf5 ffff 83f8 ff75 e789 3424 e8ef f5ff  .......u..4$....
-00001410: ff89 3c24 e8e7 f5ff ff31 c08d 6424 2c5b  ..<$.....1..d$,[
-00001420: 5e5f 5dc3 897c 240c 896c 2404 8d83 43dc  ^_]..|$..l$...C.
-00001430: ffff c704 2406 0000 0089 4424 08e8 bef4  ....$.....D$....
-00001440: ffff b8ff ffff ffeb d28b 4424 4489 4424  ..........D$D.D$
-00001450: 0ceb d58d b600 0000 008d bc27 0000 0000  ...........'....
-00001460: 5557 5653 e827 f7ff ff81 c307 2b00 008d  UWVS.'......+...
-00001470: a424 d4fb ffff 8b83 f8ff ffff 8d74 241c  .$...........t$.
-00001480: 8bac 2440 0400 008b 0089 8424 1c04 0000  ..$@.......$....
-00001490: 8d83 57dc ffff 8944 2404 8d83 59dc ffff  ..W....D$...Y...
-000014a0: 8904 24e8 28f5 ffff 85c0 89c7 751a e992  ..$.(.......u...
-000014b0: 0000 0090 8d74 2600 896c 2404 8934 24e8  .....t&..l$..4$.
-000014c0: 4cf5 ffff 85c0 7548 897c 2408 c744 2404  L.....uH.|$..D$.
-000014d0: 0004 0000 8934 24e8 44f5 ffff 85c0 75d8  .....4$.D.....u.
-000014e0: 31f6 893c 24e8 16f5 ffff 8b93 f8ff ffff  1..<$...........
-000014f0: 89f0 8b8c 241c 0400 008b 1239 d175 4a8d  ....$......9.uJ.
-00001500: a424 2c04 0000 5b5e 5f5d c390 8d74 2600  .$,...[^_]...t&.
-00001510: 8934 248d 8369 dcff ff89 4424 04e8 0ef5  .4$..i....D$....
-00001520: ffff 8904 24c7 4424 0810 0000 00c7 4424  ....$.D$......D$
-00001530: 0400 0000 00e8 06f5 ffff 3d00 8000 0089  ..........=.....
-00001540: c675 9feb 9b31 f6eb a18d b426 0000 0000  .u...1.....&....
-00001550: e81b f6ff ff8d 7426 008d bc27 0000 0000  ......t&...'....
-00001560: 5557 5653 e827 f6ff ff81 c307 2a00 008d  UWVS.'......*...
-00001570: a424 54ff ffff 8bac 24c0 0000 00c7 4424  .$T.....$.....D$
-00001580: 0400 0000 0089 2c24 e8c3 f4ff ff83 f8ff  ......,$........
-00001590: 89c6 0f84 0003 0000 31c0 8d7c 2440 b918  ........1..|$@..
-000015a0: 0000 00f3 ab89 3424 8d44 2440 8944 2404  ......4$.D$@.D$.
-000015b0: e8ab f4ff ff85 c00f 8503 0200 008b 4424  ..............D$
-000015c0: 6c89 6c24 0cc7 0424 0300 0000 8944 2434  l.l$...$.....D$4
-000015d0: 89c7 8944 2410 8d83 90dc ffff 8944 2408  ...D$........D$.
-000015e0: 8d83 f1da ffff 8944 2404 8944 2438 e80d  .......D$..D$8..
-000015f0: f3ff ffc7 4424 1400 0000 00c7 4424 1000  ....D$......D$..
-00001600: 0000 00c7 4424 0c22 0000 00c7 4424 0803  ....D$."....D$..
-00001610: 0000 0089 7c24 04c7 0424 0000 0000 e84d  ....|$...$.....M
-00001620: f4ff ff89 4424 2c83 f8ff 0f84 9a02 0000  ....D$,.........
-00001630: 8b7c 242c 8b6c 2434 c744 2404 0000 0000  .|$,.l$4.D$.....
-00001640: 893c 2489 6c24 08e8 34f4 ffff 896c 2408  .<$.l$..4....l$.
-00001650: 897c 2404 8934 24e8 34f4 ffff 8934 24e8  .|$..4$.4....4$.
-00001660: 3cf4 ffff 8b4f 200f b747 2e01 f966 85c0  <....O ..G...f..
-00001670: 0f84 7902 0000 8d04 8031 f6c7 4424 3c00  ..y......1..D$<.
-00001680: 0000 0031 ffc1 e003 c744 2430 0000 0000  ...1.....D$0....
-00001690: c744 2420 0000 0000 c744 2428 0000 0000  .D$ .....D$(....
-000016a0: 8944 2424 eb2e 6690 8b41 1031 d289 4424  .D$$..f..A.1..D$
-000016b0: 288b 4114 f771 2489 4424 2089 e884 c00f  (.A..q$.D$ .....
-000016c0: 8533 0100 0083 c628 83c7 0183 c128 3b74  .3.....(.....(;t
-000016d0: 2424 743c 8b41 0483 f80b 0f94 c289 d574  $$t<.A.........t
-000016e0: c783 f802 74c2 83f8 0375 da8b 4424 2c0f  ....t....u..D$,.
-000016f0: b740 3239 f874 ce83 c628 83c7 018b 4110  .@29.t...(....A.
-00001700: 83c1 283b 7424 2489 4424 3075 c78d 7600  ..(;t$$.D$0u..v.
-00001710: 8b4c 2428 8b74 2430 85c9 89f0 0f84 1b01  .L$(.t$0........
-00001720: 0000 8b54 2420 85d2 0f84 0f01 0000 85f6  ...T$ ..........
-00001730: 0f84 0b01 0000 8b44 242c 8b7c 2428 8b74  .......D$,.|$(.t
-00001740: 2430 01c7 01c6 8b44 2420 85c0 0f8e 2101  $0.....D$ ....!.
-00001750: 0000 31ed 89f8 89ef 89c5 eb14 8d74 2600  ..1..........t&.
-00001760: 83c7 0183 c510 3b7c 2420 0f84 0301 0000  ......;|$ ......
-00001770: 8b84 24c4 0000 0089 4424 048b 4500 01f0  ..$.....D$..E...
-00001780: 8904 24e8 28f3 ffff 85c0 75d4 8b44 2434  ..$.(.....u..D$4
-00001790: 8b75 0489 4424 048b 4424 2c89 0424 e81d  .u..D$..D$,..$..
-000017a0: f3ff ff85 f60f 84dc 0000 0089 f02b 4424  .............+D$
-000017b0: 3c8d a424 ac00 0000 5b5e 5f5d c38d 7600  <..$....[^_]..v.
-000017c0: 8944 2410 8d83 7cdc ffff 8944 2408 8d83  .D$...|....D$...
-000017d0: f1da ffff 896c 240c c704 2406 0000 0089  .....l$...$.....
-000017e0: 4424 04e8 18f1 ffff 31c0 8da4 24ac 0000  D$......1...$...
-000017f0: 005b 5e5f 5dc3 6690 8b54 242c 8b42 1c0f  .[^_].f..T$,.B..
-00001800: b76a 2c01 d066 85ed 0f84 b7fe ffff 83c5  .j,..f..........
-00001810: 01ba 0100 0000 eb0e 83c2 0183 c020 39ea  ............. 9.
-00001820: 0f84 9ffe ffff 8338 0175 ed83 7804 0075  .......8.u..x..u
-00001830: e78b 4008 8944 243c e988 feff ff8b 4424  ..@..D$<......D$
-00001840: 3089 4424 148b 4424 20c7 0424 0600 0000  0.D$..D$ ..$....
-00001850: 8944 2410 8b44 2428 8944 240c 8d83 b4dd  .D$..D$(.D$.....
-00001860: ffff 8944 2408 8b44 2438 8944 2404 e88d  ...D$..D$8.D$...
-00001870: f0ff ff8b 4424 3489 4424 048b 4424 2c89  ....D$4.D$..D$,.
-00001880: 0424 e839 f2ff ff8d a424 ac00 0000 31c0  .$.9.....$....1.
-00001890: 5b5e 5f5d c38d 7600 896c 240c 8d83 6bdc  [^_]..v..l$...k.
-000018a0: ffff 8944 2408 8d83 f1da ffff c704 2406  ...D$.........$.
-000018b0: 0000 0089 4424 04e8 44f0 ffff 8da4 24ac  ....D$..D.....$.
-000018c0: 0000 0031 c05b 5e5f 5dc3 c704 2406 0000  ...1.[^_]...$...
-000018d0: 008d 839c dcff ff89 4424 088b 4424 3889  ........D$..D$8.
-000018e0: 4424 04e8 18f0 ffff 31c0 e9fb feff ffc7  D$......1.......
-000018f0: 4424 2000 0000 0031 c0c7 4424 2800 0000  D$ ....1..D$(...
-00001900: 00e9 3bff ffff 8d76 008d bc27 0000 0000  ..;....v...'....
-00001910: 5557 5653 e877 f2ff ff81 c357 2600 008d  UWVS.w.....W&...
-00001920: 6424 d48d b3f0 ddff ff89 7424 04c7 0424  d$........t$...$
-00001930: ffff ffff e897 f1ff ff85 c089 c774 3189  .............t1.
-00001940: 4424 0c8d 83b0 dcff ff89 4424 088d 83f1  D$........D$....
-00001950: daff ffc7 0424 0400 0000 8944 2404 e89d  .....$.....D$...
-00001960: efff ffff d78d 6424 2c5b 5e5f 5dc3 6690  ......d$,[^_].f.
-00001970: 8dbb 18de ffff 893c 24e8 e2fa ffff 8944  .......<$......D
-00001980: 2410 89c5 897c 240c 8d83 c7dc ffff 8944  $....|$........D
-00001990: 2408 8d83 f1da ffff c704 2404 0000 0089  $.........$.....
-000019a0: 4424 0489 4424 18e8 54ef ffff 85ed 747d  D$..D$..T.....t}
-000019b0: 8974 2404 893c 24e8 a4fb ffff 8944 2410  .t$..<$......D$.
-000019c0: 8944 241c 8d83 dadc ffff 8944 2408 8b44  .D$........D$..D
-000019d0: 2418 8974 240c c704 2404 0000 0089 4424  $..t$...$.....D$
-000019e0: 04e8 1aef ffff 8b54 241c 85d2 7412 01d5  .......T$...t...
-000019f0: ffd5 8d64 242c 5b5e 5f5d c390 8d74 2600  ...d$,[^_]...t&.
-00001a00: 897c 2410 8d83 f3dc ffff 8944 2408 8b44  .|$........D$..D
-00001a10: 2418 8974 240c c704 2406 0000 0089 4424  $..t$...$.....D$
-00001a20: 04e8 daee ffff 31c0 e938 ffff ffc7 0424  ......1..8.....$
-00001a30: 0600 0000 8d83 3cde ffff 8944 2408 8b44  ......<....D$..D
-00001a40: 2418 8944 2404 e8b5 eeff ff31 c0e9 13ff  $..D$......1....
-00001a50: ffff 0000 456e 7465 7220 7468 7265 6164  ....Enter thread
-00001a60: 0064 6578 6c6f 6164 6572 0047 6574 2065  .dexloader.Get e
-00001a70: 6e76 2066 6169 6c65 6400 4375 7272 656e  nv failed.Curren
-00001a80: 7420 4a4e 4945 6e76 3a20 2570 006a 6176  t JNIEnv: %p.jav
-00001a90: 612f 6c61 6e67 2f43 6c61 7373 4c6f 6164  a/lang/ClassLoad
-00001aa0: 6572 0028 294c 6a61 7661 2f6c 616e 672f  er.()Ljava/lang/
-00001ab0: 436c 6173 734c 6f61 6465 723b 0067 6574  ClassLoader;.get
-00001ac0: 5379 7374 656d 436c 6173 734c 6f61 6465  SystemClassLoade
-00001ad0: 7200 6461 6c76 696b 2f73 7973 7465 6d2f  r.dalvik/system/
-00001ae0: 4465 7843 6c61 7373 4c6f 6164 6572 003c  DexClassLoader.<
-00001af0: 696e 6974 3e00 4f62 6a65 6374 2064 6578  init>.Object dex
-00001b00: 5f6c 6f61 6465 723a 2025 7000 6669 6e64  _loader: %p.find
-00001b10: 436c 6173 7300 436c 6173 7320 2573 3a20  Class.Class %s: 
-00001b20: 2570 0046 696e 6420 636c 6173 7320 2573  %p.Find class %s
-00001b30: 2066 6169 6c65 6400 4578 6974 2074 6872   failed.Exit thr
-00001b40: 6561 6400 2573 2f25 6400 4f75 7420 6669  ead.%s/%d.Out fi
-00001b50: 6c65 2064 6972 3a20 2573 0025 732f 2573  le dir: %s.%s/%s
-00001b60: 004a 4e49 456e 763a 2025 700a 0047 6574  .JNIEnv: %p..Get
-00001b70: 206a 766d 2066 6169 6c65 643a 2025 6400   jvm failed: %d.
-00001b80: 4a61 7661 564d 3a20 2570 0043 7265 6174  JavaVM: %p.Creat
-00001b90: 6520 6c6f 6164 696e 6720 7468 7265 6164  e loading thread
-00001ba0: 0063 6f70 7920 2573 2074 6f20 2573 0a00  .copy %s to %s..
-00001bb0: 7262 006f 7065 6e20 2573 2065 7272 6f72  rb.open %s error
-00001bc0: 2021 0a00 7762 0072 002f 7072 6f63 2f73   !..wb.r./proc/s
-00001bd0: 656c 662f 6d61 7073 002d 0063 616e 6e6f  elf/maps.-.canno
-00001be0: 7420 6f70 656e 2027 2573 2700 6673 7461  t open '%s'.fsta
-00001bf0: 7420 2573 2066 6169 6c65 643a 2025 6400  t %s failed: %d.
-00001c00: 2573 2073 697a 653a 2025 6400 416c 6c6f  %s size: %d.Allo
-00001c10: 6320 6d65 6d6f 7279 2066 6169 6c65 6400  c memory failed.
-00001c20: 6765 744a 4e49 456e 7620 6279 2064 6c73  getJNIEnv by dls
-00001c30: 796d 3a20 2570 004d 6f64 756c 6520 2573  ym: %p.Module %s
-00001c40: 2062 6173 653a 2025 7000 4675 6e63 7469   base: %p.Functi
-00001c50: 6f6e 2025 7320 6f66 6673 6574 3a20 3078  on %s offset: 0x
-00001c60: 2578 0046 756e 6374 696f 6e20 2573 206e  %x.Function %s n
-00001c70: 6f74 2066 6f75 6e64 2069 6e20 2573 0000  ot found in %s..
-00001c80: 284c 6a61 7661 2f6c 616e 672f 5374 7269  (Ljava/lang/Stri
-00001c90: 6e67 3b4c 6a61 7661 2f6c 616e 672f 5374  ng;Ljava/lang/St
-00001ca0: 7269 6e67 3b4c 6a61 7661 2f6c 616e 672f  ring;Ljava/lang/
-00001cb0: 5374 7269 6e67 3b4c 6a61 7661 2f6c 616e  String;Ljava/lan
-00001cc0: 672f 436c 6173 734c 6f61 6465 723b 2956  g/ClassLoader;)V
-00001cd0: 0000 0000 284c 6a61 7661 2f6c 616e 672f  ....(Ljava/lang/
-00001ce0: 5374 7269 6e67 3b29 4c6a 6176 612f 6c61  String;)Ljava/la
-00001cf0: 6e67 2f43 6c61 7373 3b00 0000 4c6f 6164  ng/Class;...Load
-00001d00: 2064 6578 2025 7320 746f 2025 732c 2061   dex %s to %s, a
-00001d10: 6e64 2063 616c 6c20 2573 2e25 7320 2573  nd call %s.%s %s
-00001d20: 0a00 0000 7379 6d74 6162 5f6f 6666 7365  ....symtab_offse
-00001d30: 743d 3078 2578 2073 796d 7461 625f 656e  t=0x%x symtab_en
-00001d40: 7472 6965 733d 3078 2578 2073 7472 7461  tries=0x%x strta
-00001d50: 625f 6f66 6673 6574 3d30 7825 7800 0000  b_offset=0x%x...
-00001d60: 5f5a 4e37 616e 6472 6f69 6431 3441 6e64  _ZN7android14And
-00001d70: 726f 6964 5275 6e74 696d 6539 6765 744a  roidRuntime9getJ
-00001d80: 4e49 456e 7645 7600 2f73 7973 7465 6d2f  NIEnvEv./system/
-00001d90: 6c69 622f 6c69 6261 6e64 726f 6964 5f72  lib/libandroid_r
-00001da0: 756e 7469 6d65 2e73 6f00 0000 4d75 7374  untime.so...Must
-00001db0: 2072 756e 2069 6e20 416e 6472 6f69 6420   run in Android 
-00001dc0: 6170 7020 7072 6f63 6573 7300 1400 0000  app process.....
-00001dd0: 0000 0000 017a 5200 017c 0801 1b0c 0404  .....zR..|......
-00001de0: 8801 0000 1400 0000 1c00 0000 24ed ffff  ............$...
-00001df0: 1300 0000 0044 0e10 4e0e 0400 1c00 0000  .....D..N.......
-00001e00: 3400 0000 dcec ffff 2400 0000 0041 0e08  4.......$....A..
-00001e10: 8302 4f0e 2052 0e08 41c3 0e04 1c00 0000  ..O. R..A.......
-00001e20: 5400 0000 0ced ffff 3600 0000 0041 0e08  T.......6....A..
-00001e30: 8302 4f0e 2064 0e08 41c3 0e04 1c00 0000  ..O. d..A.......
-00001e40: 7400 0000 2ced ffff 1b00 0000 0041 0e08  t...,........A..
-00001e50: 8302 4f0e 1049 0e08 41c3 0e04 1000 0000  ..O..I..A.......
-00001e60: 9400 0000 2ced ffff 0400 0000 0000 0000  ....,...........
-00001e70: 6800 0000 a800 0000 28ed ffff 5503 0000  h.......(...U...
-00001e80: 0041 0e08 8502 410e 0c87 0341 0e10 8604  .A....A....A....
-00001e90: 410e 1483 054f 0e60 0375 020a 0e14 43c3  A....O.`.u....C.
-00001ea0: 0e10 41c6 0e0c 41c7 0e08 41c5 0e04 420b  ..A...A...A...B.
-00001eb0: 0295 0a0e 1443 c30e 1041 c60e 0c41 c70e  .....C...A...A..
-00001ec0: 0841 c50e 0445 0b5e 0e14 43c3 0e10 41c6  .A...E.^..C...A.
-00001ed0: 0e0c 41c7 0e08 41c5 0e04 0000 4000 0000  ..A...A.....@...
-00001ee0: 1401 0000 1cf0 ffff de03 0000 0041 0e08  .............A..
-00001ef0: 8502 410e 0c87 0341 0e10 8604 410e 1483  ..A....A....A...
-00001f00: 0552 0e80 0703 2c03 0a0e 1441 c30e 1041  .R....,....A...A
-00001f10: c60e 0c41 c70e 0841 c50e 0442 0b00 0000  ...A...A...B....
-00001f20: 1c00 0000 5801 0000 b8f3 ffff 1b00 0000  ....X...........
-00001f30: 0041 0e08 8302 4f0e 1049 0e08 41c3 0e04  .A....O..I..A...
-00001f40: 1c00 0000 7801 0000 b8f3 ffff 2500 0000  ....x.......%...
-00001f50: 0041 0e08 8302 4f0e 2051 0e08 43c3 0e04  .A....O. Q..C...
-00001f60: 2000 0000 9801 0000 c8f3 ffff 3d00 0000   ...........=...
-00001f70: 0041 0e08 8302 4f0e 8001 690e 0841 c30e  .A....O...i..A..
-00001f80: 0400 0000 3c00 0000 bc01 0000 e4f3 ffff  ....<...........
-00001f90: e300 0000 0041 0e08 8502 410e 0c87 0341  .....A....A....A
-00001fa0: 0e10 8604 410e 1483 054f 0e40 029c 0a0e  ....A....O.@....
-00001fb0: 1441 c30e 1041 c60e 0c41 c70e 0841 c50e  .A...A...A...A..
-00001fc0: 0441 0b00 3c00 0000 fc01 0000 94f4 ffff  .A..<...........
-00001fd0: f500 0000 0041 0e08 8502 410e 0c87 0341  .....A....A....A
-00001fe0: 0e10 8604 410e 1483 0552 0ec0 0802 900a  ....A....R......
-00001ff0: 0e14 41c3 0e10 41c6 0e0c 41c7 0e08 41c5  ..A...A...A...A.
-00002000: 0e04 460b 8000 0000 3c02 0000 54f5 ffff  ..F.....<...T...
-00002010: a603 0000 0041 0e08 8502 410e 0c87 0341  .....A....A....A
-00002020: 0e10 8604 410e 1483 0552 0ec0 0103 4202  ....A....R....B.
-00002030: 0a0e 1441 c30e 1041 c60e 0c41 c70e 0841  ...A...A...A...A
-00002040: c50e 0444 0b71 0a0e 1441 c30e 1041 c60e  ...D.q...A...A..
-00002050: 0c41 c70e 0841 c50e 0443 0b02 960a 0e14  .A...A...C......
-00002060: 43c3 0e10 41c6 0e0c 41c7 0e08 41c5 0e04  C...A...A...A...
-00002070: 440b 6b0a 0e14 43c3 0e10 41c6 0e0c 41c7  D.k...C...A...A.
-00002080: 0e08 41c5 0e04 410b 5400 0000 c002 0000  ..A...A.T.......
-00002090: 80f8 ffff 4201 0000 0041 0e08 8502 410e  ....B....A....A.
-000020a0: 0c87 0341 0e10 8604 410e 1483 054f 0e40  ...A....A....O.@
-000020b0: 0246 0a0e 1441 c30e 1041 c60e 0c41 c70e  .F...A...A...A..
-000020c0: 0841 c50e 0443 0b02 860a 0e14 41c3 0e10  .A...C......A...
-000020d0: 41c6 0e0c 41c7 0e08 41c5 0e04 460b 0000  A...A...A...F...
-000020e0: 2400 0000 1803 0000 d8e7 ffff 2002 0000  $........... ...
-000020f0: 000e 0846 0e0c 4a0f 0b74 0478 003f 1a3b  ...F..J..t.x.?.;
-00002100: 2a32 2422 0000 0000 0000 0000 011b 033b  *2$"...........;
-00002110: bcfc ffff 0f00 0000 b4e7 ffff d4ff ffff  ................
-00002120: d4e9 ffff f0fc ffff 04ea ffff d8fc ffff  ................
-00002130: 24ea ffff 10fd ffff 64ea ffff 30fd ffff  $.......d...0...
-00002140: 84ea ffff 50fd ffff 94ea ffff 64fd ffff  ....P.......d...
-00002150: f4ed ffff d0fd ffff d4f1 ffff 14fe ffff  ................
-00002160: f4f1 ffff 34fe ffff 24f2 ffff 54fe ffff  ....4...$...T...
-00002170: 64f2 ffff 78fe ffff 54f3 ffff b8fe ffff  d...x...T.......
-00002180: 54f4 ffff f8fe ffff 04f8 ffff 7cff ffff  T...........|...
-00002190: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000021a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000021b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000021c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000021d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000021e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000021f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002230: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002240: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002250: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002260: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002270: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002280: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002290: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000022a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000022b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000022c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000022d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000022e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000022f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002300: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002310: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002320: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002330: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002340: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002350: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002370: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000023a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000023b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000023c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000023d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000023e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000023f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002400: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002410: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002420: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002430: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002440: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002450: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002460: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002470: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002480: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002490: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000024a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000024b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000024c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000024d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000024e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000024f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002500: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002510: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002520: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002530: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002540: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002550: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002560: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002570: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002580: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002590: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000025a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000025b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000025c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000025d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000025e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000025f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002600: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002610: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002620: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002630: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002640: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002650: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002660: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002670: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002680: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002690: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000026a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000026b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000026c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000026d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000026e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000026f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002700: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002710: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002720: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002730: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002740: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002750: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002760: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002770: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002780: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002790: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000027a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000027b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000027c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000027d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000027e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000027f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002800: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002810: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002820: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002830: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002840: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002850: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002860: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002870: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002880: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002890: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000028a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000028b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000028c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000028d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000028e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000028f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002900: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002910: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002920: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002930: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002940: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002950: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002960: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002970: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002980: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002990: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000029a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000029b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000029c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000029d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000029e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000029f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002a00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002a10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002a20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002a30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002a40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002a50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002a60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002a70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002a80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002a90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002aa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002ab0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002ac0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002ad0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002ae0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002af0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002b00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002b10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002b20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002b30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002b40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002b50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002b60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002b70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002b80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002b90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002ba0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002bb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002bc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002bd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002be0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002bf0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002c00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002c10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002c20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002c30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002c40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002c50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002c60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002c70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002c80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002c90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002ca0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002cb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002cc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002cd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002ce0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002cf0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002d00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002d10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002d20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002d30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002d40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002d50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002d60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002d70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002d80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002d90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002da0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002db0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002dc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002dd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002de0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002df0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002e00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002e10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002e20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002e30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002e40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002e50: 0000 0000 0000 0000 0000 0000 e00a 0000  ................
-00002e60: 0000 0000 0000 0000 0300 0000 703f 0000  ............p?..
-00002e70: 0200 0000 0801 0000 1700 0000 ac07 0000  ................
-00002e80: 1400 0000 1100 0000 1100 0000 8c07 0000  ................
-00002e90: 1200 0000 2000 0000 1300 0000 0800 0000  .... ...........
-00002ea0: faff ff6f 0300 0000 0600 0000 1401 0000  ...o............
-00002eb0: 0b00 0000 1000 0000 0500 0000 0404 0000  ................
-00002ec0: 0a00 0000 2f02 0000 0400 0000 3406 0000  ..../.......4...
-00002ed0: 0100 0000 ef01 0000 0100 0000 f901 0000  ................
-00002ee0: 0100 0000 0602 0000 0100 0000 0e02 0000  ................
-00002ef0: 0100 0000 1602 0000 0e00 0000 1f02 0000  ................
-00002f00: 1a00 0000 5c3e 0000 1c00 0000 0800 0000  ....\>..........
-00002f10: 1900 0000 643e 0000 1b00 0000 0400 0000  ....d>..........
-00002f20: 1000 0000 0000 0000 1e00 0000 0a00 0000  ................
-00002f30: fbff ff6f 0100 0000 0000 0000 0000 0000  ...o............
-00002f40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002f50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002f60: 0000 0000 0000 0000 0000 0000 a00b 0000  ................
-00002f70: 683e 0000 0000 0000 0000 0000 d608 0000  h>..............
-00002f80: e608 0000 f608 0000 0609 0000 1609 0000  ................
-00002f90: 2609 0000 3609 0000 4609 0000 5609 0000  &...6...F...V...
-00002fa0: 6609 0000 7609 0000 8609 0000 9609 0000  f...v...........
-00002fb0: a609 0000 b609 0000 c609 0000 d609 0000  ................
-00002fc0: e609 0000 f609 0000 060a 0000 160a 0000  ................
-00002fd0: 260a 0000 360a 0000 460a 0000 560a 0000  &...6...F...V...
-00002fe0: 660a 0000 760a 0000 860a 0000 960a 0000  f...v...........
-00002ff0: a60a 0000 b60a 0000 c60a 0000 d60a 0000  ................
-00003000: 0040 0000 0047 4343 3a20 2847 4e55 2920  .@...GCC: (GNU) 
-00003010: 342e 3800 0400 0000 0900 0000 0400 0000  4.8.............
-00003020: 474e 5500 676f 6c64 2031 2e31 3100 0000  GNU.gold 1.11...
-00003030: 002e 7368 7374 7274 6162 002e 6479 6e73  ..shstrtab..dyns
-00003040: 796d 002e 6479 6e73 7472 002e 6861 7368  ym..dynstr..hash
-00003050: 002e 7265 6c2e 6479 6e00 2e72 656c 2e70  ..rel.dyn..rel.p
-00003060: 6c74 002e 7465 7874 002e 726f 6461 7461  lt..text..rodata
-00003070: 002e 6568 5f66 7261 6d65 002e 6568 5f66  ..eh_frame..eh_f
-00003080: 7261 6d65 5f68 6472 002e 6669 6e69 5f61  rame_hdr..fini_a
-00003090: 7272 6179 002e 696e 6974 5f61 7272 6179  rray..init_array
-000030a0: 002e 6479 6e61 6d69 6300 2e67 6f74 002e  ..dynamic..got..
-000030b0: 676f 742e 706c 7400 2e64 6174 6100 2e62  got.plt..data..b
-000030c0: 7373 002e 636f 6d6d 656e 7400 2e6e 6f74  ss..comment..not
-000030d0: 652e 676e 752e 676f 6c64 2d76 6572 7369  e.gnu.gold-versi
-000030e0: 6f6e 0000 0000 0000 0000 0000 0000 0000  on..............
-000030f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003100: 0000 0000 0000 0000 0000 0000 0b00 0000  ................
-00003110: 0b00 0000 0200 0000 1401 0000 1401 0000  ................
-00003120: f002 0000 0200 0000 0100 0000 0400 0000  ................
-00003130: 1000 0000 1300 0000 0300 0000 0200 0000  ................
-00003140: 0404 0000 0404 0000 2f02 0000 0000 0000  ......../.......
-00003150: 0000 0000 0100 0000 0000 0000 1b00 0000  ................
-00003160: 0500 0000 0200 0000 3406 0000 3406 0000  ........4...4...
-00003170: 5801 0000 0100 0000 0000 0000 0400 0000  X...............
-00003180: 0400 0000 2100 0000 0900 0000 0200 0000  ....!...........
-00003190: 8c07 0000 8c07 0000 2000 0000 0100 0000  ........ .......
-000031a0: 0000 0000 0400 0000 0800 0000 2a00 0000  ............*...
-000031b0: 0900 0000 4200 0000 ac07 0000 ac07 0000  ....B...........
-000031c0: 0801 0000 0100 0000 0600 0000 0400 0000  ................
-000031d0: 0800 0000 2e00 0000 0100 0000 0600 0000  ................
-000031e0: c008 0000 c008 0000 2002 0000 0000 0000  ........ .......
-000031f0: 0000 0000 1000 0000 0400 0000 3300 0000  ............3...
-00003200: 0100 0000 0600 0000 e00a 0000 e00a 0000  ................
-00003210: 720f 0000 0000 0000 0000 0000 1000 0000  r...............
-00003220: 0000 0000 3900 0000 0100 0000 3200 0000  ....9.......2...
-00003230: 541a 0000 541a 0000 7803 0000 0000 0000  T...T...x.......
-00003240: 0000 0000 0400 0000 0100 0000 4100 0000  ............A...
-00003250: 0100 0000 0200 0000 cc1d 0000 cc1d 0000  ................
-00003260: 4003 0000 0000 0000 0000 0000 0400 0000  @...............
-00003270: 0000 0000 4b00 0000 0100 0000 0200 0000  ....K...........
-00003280: 0c21 0000 0c21 0000 8400 0000 0000 0000  .!...!..........
-00003290: 0000 0000 0400 0000 0000 0000 5900 0000  ............Y...
-000032a0: 0f00 0000 0300 0000 5c3e 0000 5c2e 0000  ........\>..\...
-000032b0: 0800 0000 0000 0000 0000 0000 0400 0000  ................
-000032c0: 0000 0000 6500 0000 0e00 0000 0300 0000  ....e...........
-000032d0: 643e 0000 642e 0000 0400 0000 0000 0000  d>..d...........
-000032e0: 0000 0000 0100 0000 0000 0000 7100 0000  ............q...
-000032f0: 0600 0000 0300 0000 683e 0000 682e 0000  ........h>..h...
-00003300: 0001 0000 0200 0000 0000 0000 0400 0000  ................
-00003310: 0800 0000 7a00 0000 0100 0000 0300 0000  ....z...........
-00003320: 683f 0000 682f 0000 0800 0000 0000 0000  h?..h/..........
-00003330: 0000 0000 0400 0000 0000 0000 7f00 0000  ................
-00003340: 0100 0000 0300 0000 703f 0000 702f 0000  ........p?..p/..
-00003350: 9000 0000 0000 0000 0000 0000 0400 0000  ................
-00003360: 0000 0000 8800 0000 0100 0000 0300 0000  ................
-00003370: 0040 0000 0030 0000 0400 0000 0000 0000  .@...0..........
-00003380: 0000 0000 0400 0000 0000 0000 8e00 0000  ................
-00003390: 0800 0000 0300 0000 0440 0000 0430 0000  .........@...0..
-000033a0: 0000 0000 0000 0000 0000 0000 0100 0000  ................
-000033b0: 0000 0000 9300 0000 0100 0000 3000 0000  ............0...
-000033c0: 0000 0000 0430 0000 1000 0000 0000 0000  .....0..........
-000033d0: 0000 0000 0100 0000 0100 0000 9c00 0000  ................
-000033e0: 0700 0000 0000 0000 0000 0000 1430 0000  .............0..
-000033f0: 1c00 0000 0000 0000 0000 0000 0400 0000  ................
-00003400: 0000 0000 0100 0000 0300 0000 0000 0000  ................
-00003410: 0000 0000 3030 0000 b300 0000 0000 0000  ....00..........
-00003420: 0000 0000 0100 0000 0000 0000            ............
+00000010: 0300 0300 0100 0000 9010 0000 3400 0000  ............4...
+00000020: 8c44 0000 0000 0000 3400 2000 0800 2800  .D......4. ...(.
+00000030: 1800 1700 0600 0000 3400 0000 3400 0000  ........4...4...
+00000040: 3400 0000 0001 0000 0001 0000 0400 0000  4...............
+00000050: 0400 0000 0300 0000 3401 0000 3401 0000  ........4...4...
+00000060: 3401 0000 1300 0000 1300 0000 0400 0000  4...............
+00000070: 0100 0000 0100 0000 0000 0000 0000 0000  ................
+00000080: 0000 0000 583c 0000 583c 0000 0500 0000  ....X<..X<......
+00000090: 0010 0000 0100 0000 143e 0000 144e 0000  .........>...N..
+000000a0: 144e 0000 6c05 0000 7405 0000 0600 0000  .N..l...t.......
+000000b0: 0010 0000 0200 0000 2c3e 0000 2c4e 0000  ........,>..,N..
+000000c0: 2c4e 0000 0801 0000 0801 0000 0600 0000  ,N..............
+000000d0: 0400 0000 50e5 7464 5c3b 0000 5c3b 0000  ....P.td\;..\;..
+000000e0: 5c3b 0000 fc00 0000 fc00 0000 0400 0000  \;..............
+000000f0: 0400 0000 51e5 7464 0000 0000 0000 0000  ....Q.td........
+00000100: 0000 0000 0000 0000 0000 0000 0600 0000  ................
+00000110: 0000 0000 52e5 7464 143e 0000 144e 0000  ....R.td.>...N..
+00000120: 144e 0000 ec01 0000 ec01 0000 0600 0000  .N..............
+00000130: 0400 0000 2f73 7973 7465 6d2f 6269 6e2f  ..../system/bin/
+00000140: 6c69 6e6b 6572 0000 0000 0000 0000 0000  linker..........
+00000150: 0000 0000 0000 0000 0100 0000 0000 0000  ................
+00000160: 0000 0000 1200 0000 0d00 0000 0000 0000  ................
+00000170: 0000 0000 1200 0000 1a00 0000 0000 0000  ................
+00000180: 0000 0000 1200 0000 2b00 0000 0000 0000  ........+.......
+00000190: 0000 0000 1100 0000 3d00 0000 0000 0000  ........=.......
+000001a0: 0000 0000 1200 0000 5300 0000 0000 0000  ........S.......
+000001b0: 0000 0000 1200 0000 5800 0000 0000 0000  ........X.......
+000001c0: 0000 0000 1200 0000 5f00 0000 0000 0000  ........_.......
+000001d0: 0000 0000 1200 0000 7300 0000 0000 0000  ........s.......
+000001e0: 0000 0000 1200 0000 7a00 0000 0000 0000  ........z.......
+000001f0: 0000 0000 1200 0000 8100 0000 0000 0000  ................
+00000200: 0000 0000 1200 0000 8800 0000 0000 0000  ................
+00000210: 0000 0000 1200 0000 8f00 0000 0000 0000  ................
+00000220: 0000 0000 1200 0000 9700 0000 0000 0000  ................
+00000230: 0000 0000 1200 0000 a000 0000 0000 0000  ................
+00000240: 0000 0000 1200 0000 a600 0000 0000 0000  ................
+00000250: 0000 0000 1200 0000 ad00 0000 0000 0000  ................
+00000260: 0000 0000 1200 0000 b300 0000 0000 0000  ................
+00000270: 0000 0000 1200 0000 ba00 0000 0000 0000  ................
+00000280: 0000 0000 1200 0000 c100 0000 0000 0000  ................
+00000290: 0000 0000 1200 0000 c900 0000 0000 0000  ................
+000002a0: 0000 0000 1200 0000 ce00 0000 0000 0000  ................
+000002b0: 0000 0000 1200 0000 d400 0000 0000 0000  ................
+000002c0: 0000 0000 1200 0000 db00 0000 0000 0000  ................
+000002d0: 0000 0000 1200 0000 e200 0000 0000 0000  ................
+000002e0: 0000 0000 1200 0000 e700 0000 0000 0000  ................
+000002f0: 0000 0000 1200 0000 ed00 0000 0000 0000  ................
+00000300: 0000 0000 1200 0000 f400 0000 0000 0000  ................
+00000310: 0000 0000 1200 0000 f900 0000 0000 0000  ................
+00000320: 0000 0000 1100 0000 fe00 0000 0000 0000  ................
+00000330: 0000 0000 1200 0000 0601 0000 0000 0000  ................
+00000340: 0000 0000 1200 0000 0d01 0000 0000 0000  ................
+00000350: 0000 0000 1200 0000 1301 0000 0000 0000  ................
+00000360: 0000 0000 1200 0000 1b01 0000 0000 0000  ................
+00000370: 0000 0000 1200 0000 2301 0000 0000 0000  ........#.......
+00000380: 0000 0000 1200 0000 2c01 0000 0000 0000  ........,.......
+00000390: 0000 0000 1200 0000 3401 0000 0000 0000  ........4.......
+000003a0: 0000 0000 1200 0000 3b01 0000 0000 0000  ........;.......
+000003b0: 0000 0000 1200 0000 4401 0000 0000 0000  ........D.......
+000003c0: 0000 0000 1200 0000 4a01 0000 0000 0000  ........J.......
+000003d0: 0000 0000 1200 0000 5601 0000 0000 0000  ........V.......
+000003e0: 0000 0000 1100 0000 5d01 0000 0000 0000  ........].......
+000003f0: 0000 0000 1200 0000 6301 0000 0000 0000  ........c.......
+00000400: 0000 0000 1200 0000 6801 0000 8053 0000  ........h....S..
+00000410: 0000 0000 1000 f1ff 6f01 0000 8053 0000  ........o....S..
+00000420: 0000 0000 1000 f1ff 7b01 0000 8853 0000  ........{....S..
+00000430: 0000 0000 1000 f1ff 005f 5f6c 6962 635f  .........__libc_
+00000440: 696e 6974 005f 5f63 7861 5f61 7465 7869  init.__cxa_atexi
+00000450: 7400 5f5f 7374 6163 6b5f 6368 6b5f 6661  t.__stack_chk_fa
+00000460: 696c 005f 5f73 7461 636b 5f63 686b 5f67  il.__stack_chk_g
+00000470: 7561 7264 005f 5f73 7973 7465 6d5f 7072  uard.__system_pr
+00000480: 6f70 6572 7479 5f67 6574 0061 746f 6900  operty_get.atoi.
+00000490: 7072 696e 7466 005f 5f61 6e64 726f 6964  printf.__android
+000004a0: 5f6c 6f67 5f70 7269 6e74 0070 7472 6163  _log_print.ptrac
+000004b0: 6500 6d65 6d63 7079 0073 7472 6c65 6e00  e.memcpy.strlen.
+000004c0: 7065 7272 6f72 0077 6169 7470 6964 0073  perror.waitpid.s
+000004d0: 6e70 7269 6e74 6600 666f 7065 6e00 7374  nprintf.fopen.st
+000004e0: 7273 7472 0066 6765 7473 0066 636c 6f73  rstr.fgets.fclos
+000004f0: 6500 7374 7274 6f6b 0073 7472 746f 756c  e.strtok.strtoul
+00000500: 006f 7065 6e00 6673 7461 7400 6d61 6c6c  .open.fstat.mall
+00000510: 6f63 006d 656d 7365 7400 7265 6164 0063  oc.memset.read.c
+00000520: 6c6f 7365 0073 7472 636d 7000 6672 6565  lose.strcmp.free
+00000530: 005f 5f73 4600 6670 7269 6e74 6600 646c  .__sF.fprintf.dl
+00000540: 6f70 656e 0064 6c73 796d 006f 7065 6e64  open.dlsym.opend
+00000550: 6972 0072 6561 6464 6972 0063 6c6f 7365  ir.readdir.close
+00000560: 6469 7200 7370 7269 6e74 6600 6677 7269  dir.sprintf.fwri
+00000570: 7465 0072 6561 646c 696e 6b00 6c73 7461  te.readlink.lsta
+00000580: 7400 6765 746f 7074 5f6c 6f6e 6700 6f70  t.getopt_long.op
+00000590: 7461 7267 0066 7075 7463 0070 7574 7300  targ.fputc.puts.
+000005a0: 5f65 6461 7461 005f 5f62 7373 5f73 7461  _edata.__bss_sta
+000005b0: 7274 005f 656e 6400 6c69 626c 6f67 2e73  rt._end.liblog.s
+000005c0: 6f00 6c69 6273 7464 632b 2b2e 736f 006c  o.libstdc++.so.l
+000005d0: 6962 6d2e 736f 006c 6962 632e 736f 006c  ibm.so.libc.so.l
+000005e0: 6962 646c 2e73 6f00 2500 0000 2f00 0000  ibdl.so.%.../...
+000005f0: 0000 0000 1f00 0000 2600 0000 0000 0000  ........&.......
+00000600: 0000 0000 0000 0000 2000 0000 0000 0000  ........ .......
+00000610: 0000 0000 0000 0000 1100 0000 1600 0000  ................
+00000620: 0200 0000 0000 0000 1300 0000 2500 0000  ............%...
+00000630: 1a00 0000 1400 0000 2c00 0000 2400 0000  ........,...$...
+00000640: 0000 0000 1900 0000 0600 0000 1700 0000  ................
+00000650: 0000 0000 1d00 0000 0000 0000 2800 0000  ............(...
+00000660: 2700 0000 0e00 0000 1000 0000 2e00 0000  '...............
+00000670: 2a00 0000 2200 0000 0000 0000 2d00 0000  *...".......-...
+00000680: 2900 0000 0000 0000 0000 0000 0000 0000  )...............
+00000690: 0000 0000 0000 0000 0000 0000 0100 0000  ................
+000006a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000006b0: 0000 0000 0700 0000 0000 0000 0b00 0000  ................
+000006c0: 0000 0000 0300 0000 0000 0000 0c00 0000  ................
+000006d0: 0f00 0000 0d00 0000 0800 0000 0400 0000  ................
+000006e0: 0000 0000 0000 0000 1500 0000 0000 0000  ................
+000006f0: 0000 0000 0000 0000 0500 0000 0900 0000  ................
+00000700: 1b00 0000 0000 0000 1e00 0000 2100 0000  ............!...
+00000710: 1200 0000 0000 0000 2300 0000 0a00 0000  ........#.......
+00000720: 0000 0000 0000 0000 0000 0000 1800 0000  ................
+00000730: 0000 0000 2b00 0000 0000 0000 1c00 0000  ....+...........
+00000740: 344f 0000 0800 0000 384f 0000 0800 0000  4O......8O......
+00000750: 3c4f 0000 0800 0000 404f 0000 0800 0000  <O......@O......
+00000760: 0050 0000 0800 0000 1050 0000 0800 0000  .P.......P......
+00000770: 2050 0000 0800 0000 3050 0000 0800 0000   P......0P......
+00000780: 4050 0000 0800 0000 444f 0000 0604 0000  @P......DO......
+00000790: 484f 0000 061d 0000 4c4f 0000 061f 0000  HO......LO......
+000007a0: 504f 0000 0629 0000 604f 0000 0701 0000  PO...)..`O......
+000007b0: 644f 0000 0702 0000 684f 0000 0703 0000  dO......hO......
+000007c0: 6c4f 0000 0705 0000 704f 0000 0706 0000  lO......pO......
+000007d0: 744f 0000 0707 0000 784f 0000 0708 0000  tO......xO......
+000007e0: 7c4f 0000 0709 0000 804f 0000 070a 0000  |O.......O......
+000007f0: 844f 0000 070b 0000 884f 0000 070c 0000  .O.......O......
+00000800: 8c4f 0000 070d 0000 904f 0000 070e 0000  .O.......O......
+00000810: 944f 0000 070f 0000 984f 0000 0710 0000  .O.......O......
+00000820: 9c4f 0000 0711 0000 a04f 0000 0712 0000  .O.......O......
+00000830: a44f 0000 0713 0000 a84f 0000 0714 0000  .O.......O......
+00000840: ac4f 0000 0715 0000 b04f 0000 0716 0000  .O.......O......
+00000850: b44f 0000 0717 0000 b84f 0000 0718 0000  .O.......O......
+00000860: bc4f 0000 0719 0000 c04f 0000 071a 0000  .O.......O......
+00000870: c44f 0000 071b 0000 c84f 0000 071c 0000  .O.......O......
+00000880: cc4f 0000 071e 0000 d04f 0000 071f 0000  .O.......O......
+00000890: d44f 0000 0720 0000 d84f 0000 0721 0000  .O... ...O...!..
+000008a0: dc4f 0000 0722 0000 e04f 0000 0723 0000  .O..."...O...#..
+000008b0: e44f 0000 0724 0000 e84f 0000 0725 0000  .O...$...O...%..
+000008c0: ec4f 0000 0726 0000 f04f 0000 0727 0000  .O...&...O...'..
+000008d0: f44f 0000 0728 0000 f84f 0000 072a 0000  .O...(...O...*..
+000008e0: fc4f 0000 072b 0000 0000 0000 0000 0000  .O...+..........
+000008f0: ffb3 0400 0000 ffa3 0800 0000 0000 0000  ................
+00000900: ffa3 0c00 0000 6800 0000 00e9 e0ff ffff  ......h.........
+00000910: ffa3 1000 0000 6808 0000 00e9 d0ff ffff  ......h.........
+00000920: ffa3 1400 0000 6810 0000 00e9 c0ff ffff  ......h.........
+00000930: ffa3 1800 0000 6818 0000 00e9 b0ff ffff  ......h.........
+00000940: ffa3 1c00 0000 6820 0000 00e9 a0ff ffff  ......h ........
+00000950: ffa3 2000 0000 6828 0000 00e9 90ff ffff  .. ...h(........
+00000960: ffa3 2400 0000 6830 0000 00e9 80ff ffff  ..$...h0........
+00000970: ffa3 2800 0000 6838 0000 00e9 70ff ffff  ..(...h8....p...
+00000980: ffa3 2c00 0000 6840 0000 00e9 60ff ffff  ..,...h@....`...
+00000990: ffa3 3000 0000 6848 0000 00e9 50ff ffff  ..0...hH....P...
+000009a0: ffa3 3400 0000 6850 0000 00e9 40ff ffff  ..4...hP....@...
+000009b0: ffa3 3800 0000 6858 0000 00e9 30ff ffff  ..8...hX....0...
+000009c0: ffa3 3c00 0000 6860 0000 00e9 20ff ffff  ..<...h`.... ...
+000009d0: ffa3 4000 0000 6868 0000 00e9 10ff ffff  ..@...hh........
+000009e0: ffa3 4400 0000 6870 0000 00e9 00ff ffff  ..D...hp........
+000009f0: ffa3 4800 0000 6878 0000 00e9 f0fe ffff  ..H...hx........
+00000a00: ffa3 4c00 0000 6880 0000 00e9 e0fe ffff  ..L...h.........
+00000a10: ffa3 5000 0000 6888 0000 00e9 d0fe ffff  ..P...h.........
+00000a20: ffa3 5400 0000 6890 0000 00e9 c0fe ffff  ..T...h.........
+00000a30: ffa3 5800 0000 6898 0000 00e9 b0fe ffff  ..X...h.........
+00000a40: ffa3 5c00 0000 68a0 0000 00e9 a0fe ffff  ..\...h.........
+00000a50: ffa3 6000 0000 68a8 0000 00e9 90fe ffff  ..`...h.........
+00000a60: ffa3 6400 0000 68b0 0000 00e9 80fe ffff  ..d...h.........
+00000a70: ffa3 6800 0000 68b8 0000 00e9 70fe ffff  ..h...h.....p...
+00000a80: ffa3 6c00 0000 68c0 0000 00e9 60fe ffff  ..l...h.....`...
+00000a90: ffa3 7000 0000 68c8 0000 00e9 50fe ffff  ..p...h.....P...
+00000aa0: ffa3 7400 0000 68d0 0000 00e9 40fe ffff  ..t...h.....@...
+00000ab0: ffa3 7800 0000 68d8 0000 00e9 30fe ffff  ..x...h.....0...
+00000ac0: ffa3 7c00 0000 68e0 0000 00e9 20fe ffff  ..|...h..... ...
+00000ad0: ffa3 8000 0000 68e8 0000 00e9 10fe ffff  ......h.........
+00000ae0: ffa3 8400 0000 68f0 0000 00e9 00fe ffff  ......h.........
+00000af0: ffa3 8800 0000 68f8 0000 00e9 f0fd ffff  ......h.........
+00000b00: ffa3 8c00 0000 6800 0100 00e9 e0fd ffff  ......h.........
+00000b10: ffa3 9000 0000 6808 0100 00e9 d0fd ffff  ......h.........
+00000b20: ffa3 9400 0000 6810 0100 00e9 c0fd ffff  ......h.........
+00000b30: ffa3 9800 0000 6818 0100 00e9 b0fd ffff  ......h.........
+00000b40: ffa3 9c00 0000 6820 0100 00e9 a0fd ffff  ......h ........
+00000b50: ffa3 a000 0000 6828 0100 00e9 90fd ffff  ......h(........
+00000b60: ffa3 a400 0000 6830 0100 00e9 80fd ffff  ......h0........
+00000b70: ffa3 a800 0000 6838 0100 00e9 70fd ffff  ......h8....p...
+00000b80: 55b9 1800 0000 89e5 5756 53e8 bb05 0000  U.......WVS.....
+00000b90: 81c3 c443 0000 83e4 f08d b3ac 0000 008d  ...C............
+00000ba0: a424 30ff ffff 8d93 2c03 0000 8954 2438  .$0.....,....T$8
+00000bb0: 8d7c 2470 897c 243c f3a5 8914 248d bb2c  .|$p.|$<....$..,
+00000bc0: 0200 0089 4c24 348d b32c 0100 00e8 fe20  ....L$4..,..... 
+00000bd0: 0000 893c 24e8 f620 0000 8934 24e8 ee20  ...<$.. ...4$.. 
+00000be0: 0000 8b54 2438 8d8b 9be0 ffff 890c 2489  ...T$8........$.
+00000bf0: 4c24 3889 5424 0489 5424 30e8 50fd ffff  L$8.T$..T$0.P...
+00000c00: 8b54 2430 8b4c 2438 c704 2403 0000 0089  .T$0.L$8..$.....
+00000c10: 5424 0c8d 9326 deff ff89 4c24 0889 5424  T$...&....L$..T$
+00000c20: 0489 5424 38e8 36fd ffff 897c 2404 8d93  ..T$8.6....|$...
+00000c30: ade0 ffff 8914 2489 5424 30e8 10fd ffff  ......$.T$0.....
+00000c40: 8b54 2430 897c 240c 8dbb c1e0 ffff c704  .T$0.|$.........
+00000c50: 2403 0000 0089 5424 088b 5424 3889 5424  $.....T$..T$8.T$
+00000c60: 04e8 fafc ffff 8974 2404 893c 24e8 defc  .......t$..<$...
+00000c70: ffff 8b54 2438 8974 240c 8db3 00e1 ffff  ...T$8.t$.......
+00000c80: 897c 2408 8d7c 2448 c704 2403 0000 0089  .|$..|$H..$.....
+00000c90: 5424 04e8 c8fc ffff 8b44 2434 b90a 0000  T$.......D$4....
+00000ca0: 0089 7c24 24c7 4424 2c00 0000 00c7 4424  ..|$$.D$,.....D$
+00000cb0: 3400 0000 00c7 4424 3000 0000 00c7 4424  4.....D$0.....D$
+00000cc0: 2800 0000 00f3 abbf ffff ffff 8b44 243c  (............D$<
+00000cd0: c744 2410 0000 0000 8974 2408 8944 240c  .D$......t$..D$.
+00000ce0: 8b45 0c89 4424 048b 4508 8904 24e8 5efe  .E..D$..E...$.^.
+00000cf0: ffff 83f8 ff0f 8426 0100 0083 e850 83f8  .......&.....P..
+00000d00: 200f 87cf 0000 008b 8483 e8e4 ffff 01d8   ...............
+00000d10: ffe0 8b83 fcff ffff 83c9 ff8b 1031 c089  .............1..
+00000d20: d7f2 ae89 c8f7 d089 c731 c083 ef01 eb13  .........1......
+00000d30: 0fb6 0c02 83e9 3080 f909 0f87 b600 0000  ......0.........
+00000d40: 83c0 0139 f875 e989 1424 e8f1 fbff ff89  ...9.u...$......
+00000d50: c7e9 76ff ffff 8b83 fcff ffff 8b00 8944  ..v............D
+00000d60: 2430 e965 ffff ff8b 83f4 ffff ffc7 4424  $0.e..........D$
+00000d70: 0898 0000 00c7 4424 0401 0000 0005 a800  ......D$........
+00000d80: 0000 8944 240c 8d83 fce3 ffff 8904 24e8  ...D$.........$.
+00000d90: 8cfd ffff 31c0 8d65 f45b 5e5f 5dc3 8b83  ....1..e.[^_]...
+00000da0: fcff ffff 8b00 8944 242c e91d ffff ff83  .......D$,......
+00000db0: 7c24 3409 0f8f 8f01 0000 8b83 fcff ffff  |$4.............
+00000dc0: 8b54 2434 8b00 8944 9448 8d42 0189 4424  .T$4...D.H.B..D$
+00000dd0: 34e9 f6fe ffff 8b83 f4ff ffff c704 240a  4.............$.
+00000de0: 0000 0005 a800 0000 8944 2404 e86f fdff  .........D$..o..
+00000df0: ff83 c8ff eba0 39c7 0f86 49ff ffff 8914  ......9...I.....
+00000e00: 2489 5424 28e8 4611 0000 85c0 89c7 8b54  $.T$(.F........T
+00000e10: 2428 0f88 6601 0000 8954 2428 e9ab feff  $(..f....T$(....
+00000e20: ff85 ff0f 8886 0100 008b 4424 2885 c074  ..........D$(..t
+00000e30: 3a89 7c24 088d b328 e1ff ff89 4424 0489  :.|$...(....D$..
+00000e40: 3424 e809 fbff ff8b 4424 2889 7c24 1089  4$......D$(.|$..
+00000e50: 7424 0889 4424 0c8b 4424 38c7 0424 0300  t$..D$..D$8..$..
+00000e60: 0000 8944 2404 e8f5 faff ff83 7c24 3000  ...D$.......|$0.
+00000e70: 0f84 be01 0000 837c 242c 000f 8463 0100  .......|$,...c..
+00000e80: 008d 833c e1ff ff89 0424 e8e1 fcff ffc7  ...<.....$......
+00000e90: 0424 0300 0000 8d83 52e1 ffff 8944 2408  .$......R....D$.
+00000ea0: 8b44 2438 8944 2404 e8b3 faff ff8b 4424  .D$8.D$.......D$
+00000eb0: 34c7 4424 1401 0000 0089 3c24 8944 2410  4.D$......<$.D$.
+00000ec0: 8b44 2424 8944 240c 8b44 242c 8944 2408  .D$$.D$..D$,.D$.
+00000ed0: 8b44 2430 8944 2404 e8a3 1600 0085 c089  .D$0.D$.........
+00000ee0: c675 338d 8369 e1ff ff89 0424 e87f fcff  .u3..i.....$....
+00000ef0: ffc7 0424 0300 0000 8d83 7de1 ffff 8944  ...$......}....D
+00000f00: 2408 8b44 2438 8944 2404 e851 faff ff31  $..D$8.D$..Q...1
+00000f10: c0e9 80fe ffff 8d83 92e1 ffff 8904 24e8  ..............$.
+00000f20: 4cfc ffff c704 2403 0000 008d 83a5 e1ff  L.....$.........
+00000f30: ff89 4424 088b 4424 3889 4424 04e8 1efa  ..D$..D$8.D$....
+00000f40: ffff 89f0 e94d feff ff8b 83f4 ffff ffc7  .....M..........
+00000f50: 4424 0815 0000 00c7 4424 0401 0000 0005  D$......D$......
+00000f60: a800 0000 8944 240c 8d83 eae0 ffff 8904  .....D$.........
+00000f70: 24e8 aafb ffff 83c8 ffe9 18fe ffff 8b83  $...............
+00000f80: fcff ffff 8b00 8944 2408 8d83 d4e0 ffff  .......D$.......
+00000f90: 8944 2404 8b83 f4ff ffff 05a8 0000 0089  .D$.............
+00000fa0: 0424 e809 fbff ff83 c8ff e9e7 fdff ff8b  .$..............
+00000fb0: 83f4 ffff ffc7 4424 081d 0000 00c7 4424  ......D$......D$
+00000fc0: 0401 0000 0005 a800 0000 8944 240c 8d83  ...........D$...
+00000fd0: 0ae1 ffff 8904 24e8 44fb ffff 83c8 ffe9  ......$.D.......
+00000fe0: b2fd ffff 8b44 2430 8944 2408 8d83 bce4  .....D$0.D$.....
+00000ff0: ffff 8944 2404 8b83 f4ff ffff 8db0 a800  ...D$...........
+00001000: 0000 8934 24e8 a6fa ffff 8974 240c 8d83  ...4$......t$...
+00001010: fce3 ffff c744 2408 9800 0000 c744 2404  .....D$......D$.
+00001020: 0100 0000 8904 24e8 f4fa ffff 83c8 ffe9  ......$.........
+00001030: 62fd ffff 8b83 f4ff ffff c744 2408 2300  b..........D$.#.
+00001040: 0000 c744 2404 0100 0000 8db0 a800 0000  ...D$...........
+00001050: 8d83 98e4 ffff 8974 240c 8904 24e8 befa  .......t$...$...
+00001060: ffff eba6 0000 0000 0000 0000 0000 0000  ................
+00001070: 8d64 24f4 8b44 2410 85c0 7402 ffd0 8d64  .d$..D$...t....d
+00001080: 240c c38d b600 0000 008d bc27 0000 0000  $..........'....
+00001090: 5589 e553 e8b2 0000 0081 c3bb 3e00 0083  U..S........>...
+000010a0: e4f0 8d64 24e0 8b83 e0ff ffff c744 2404  ...d$........D$.
+000010b0: 0000 0000 8944 2414 8b83 e4ff ffff 8944  .....D$........D
+000010c0: 2418 8b83 e8ff ffff 8944 241c 8d44 2414  $........D$..D$.
+000010d0: 8944 240c 8b83 ecff ffff 8944 2408 8d45  .D$........D$..E
+000010e0: 0489 0424 e817 f8ff ff8d b426 0000 0000  ...$.......&....
+000010f0: 53e8 5500 0000 81c3 5e3e 0000 8d64 24e8  S.U.....^>...d$.
+00001100: 8d83 2c04 0000 8944 2408 8b44 2420 8944  ..,....D$..D$ .D
+00001110: 2404 8d83 1cc1 ffff 8904 24e8 f0f7 ffff  $.........$.....
+00001120: 8d64 2418 5bc3 8d76 008d bc27 0000 0000  .d$.[..v...'....
+00001130: 53e8 1500 0000 81c3 1e3e 0000 8d64 24f8  S........>...d$.
+00001140: e8db f7ff ff8d 6424 085b c38b 1c24 c390  ......d$.[...$..
+00001150: 5756 53e8 f3ff ffff 81c3 fc3d 0000 8d64  WVS........=...d
+00001160: 24e0 8bb3 f0ff ffff 8b06 8944 241c 8b83  $..........D$...
+00001170: 3004 0000 85c0 7577 8d7c 2412 8d83 f4dd  0.....uw.|$.....
+00001180: ffff 897c 2404 8904 24c7 4424 1200 0000  ...|$...$.D$....
+00001190: 00c7 4424 1600 0000 0066 c744 241a 0000  ..D$.....f.D$...
+000011a0: e88b f7ff ff89 3c24 8dbb 09de ffff e88d  ......<$........
+000011b0: f7ff ff89 4424 0489 3c24 8983 3004 0000  ....D$..<$..0...
+000011c0: e88b f7ff ff8b 8330 0400 0089 7c24 08c7  .......0....|$..
+000011d0: 0424 0300 0000 8944 240c 8d83 26de ffff  .$.....D$...&...
+000011e0: 8944 2404 e877 f7ff ff8b 8330 0400 008b  .D$..w.....0....
+000011f0: 4c24 1c8b 1639 d175 088d 6424 205b 5e5f  L$...9.u..d$ [^_
+00001200: c3e8 2aff ffff 8d76 008d bc27 0000 0000  ..*....v...'....
+00001210: 5557 5653 e832 ffff ff81 c33b 3d00 008d  UWVS.2.....;=...
+00001220: 6424 c48b 6c24 5c89 e883 e003 c1ed 0289  d$..l$\.........
+00001230: 4424 1c89 6c24 1874 588b 7c24 5831 f68b  D$..l$.tX.|$X1..
+00001240: 6c24 548d b600 0000 008d bc27 0000 0000  l$T........'....
+00001250: 8b44 2450 83c6 0189 6c24 0883 c704 c744  .D$P....l$.....D
+00001260: 240c 0000 0000 83c5 04c7 0424 0100 0000  $..........$....
+00001270: 8944 2404 e8f7 f6ff ff89 47fc 3b74 2418  .D$.......G.;t$.
+00001280: 8944 242c 75ca c1e6 0201 7424 5401 7424  .D$,u.....t$T.t$
+00001290: 588b 4424 1c85 c074 448b 4424 54c7 4424  X.D$...tD.D$T.D$
+000012a0: 0c00 0000 00c7 0424 0100 0000 8944 2408  .......$.....D$.
+000012b0: 8b44 2450 8944 2404 e8b3 f6ff ff89 4424  .D$P.D$.......D$
+000012c0: 2c8d 4424 2c8b 5424 1c89 4424 048b 4424  ,.D$,.T$..D$..D$
+000012d0: 5889 5424 0889 0424 e8a3 f6ff ff8d 6424  X.T$...$......d$
+000012e0: 3c31 c05b 5e5f 5dc3 908d b426 0000 0000  <1.[^_]....&....
+000012f0: 5557 5653 e852 feff ff81 c35b 3c00 008d  UWVS.R.....[<...
+00001300: 6424 c48b 4424 5c89 c283 e203 c1e8 0289  d$..D$\.........
+00001310: 5424 1c89 4424 1474 6a8b 7c24 588d 4424  T$..D$.tj.|$X.D$
+00001320: 2c8b 6c24 5431 f689 4424 1889 f889 ef89  ,.l$T1..D$......
+00001330: c5eb 0d90 9090 9090 9090 9090 9090 9090  ................
+00001340: 8b45 0083 c601 8b4c 2418 83c5 0489 018b  .E.....L$.......
+00001350: 4424 2c89 7c24 0883 c704 c704 2404 0000  D$,.|$......$...
+00001360: 0089 4424 0c8b 4424 5089 4424 04e8 fef5  ..D$..D$P.D$....
+00001370: ffff 3b74 2414 75c8 c1e6 0201 7424 5401  ..;t$.u.....t$T.
+00001380: 7424 588b 4424 1c85 c075 0d8d 6424 3c31  t$X.D$...u..d$<1
+00001390: c05b 5e5f 5dc3 6690 8b44 2454 c744 240c  .[^_].f..D$T.D$.
+000013a0: 0000 0000 c704 2401 0000 0089 4424 088b  ......$.....D$..
+000013b0: 4424 5089 4424 04e8 b4f5 ffff 8944 242c  D$P.D$.......D$,
+000013c0: 8d54 242c 8b4c 241c 31c0 8b74 2458 89d7  .T$,.L$.1..t$X..
+000013d0: 0fb6 1406 8814 0783 c001 39c8 75f2 8b44  ..........9.u..D
+000013e0: 242c c704 2404 0000 0089 4424 0c8b 4424  $,..$.....D$..D$
+000013f0: 5489 4424 088b 4424 5089 4424 04e8 6ef5  T.D$..D$P.D$..n.
+00001400: ffff 8d64 243c 31c0 5b5e 5f5d c38d 7600  ...d$<1.[^_]..v.
+00001410: 5557 5653 e832 fdff ff81 c33b 3b00 008d  UWVS.2.....;;...
+00001420: 6424 d48d ab2d deff ff8b 7424 488b 7c24  d$...-....t$H.|$
+00001430: 4489 3424 e857 f5ff ff89 4424 0889 7424  D.4$.W....D$..t$
+00001440: 0c89 7c24 0489 2c24 e803 f5ff ff89 3424  ..|$..,$......4$
+00001450: e83b f5ff ff89 4424 108d 8326 deff ff89  .;....D$...&....
+00001460: 7424 1489 7c24 0c89 6c24 08c7 0424 0300  t$..|$..l$...$..
+00001470: 0000 8944 2404 e8e5 f4ff ff89 3424 e80d  ...D$.......4$..
+00001480: f5ff ff89 7424 0883 c001 8944 240c 8b44  ....t$.....D$..D
+00001490: 2440 897c 2404 8904 24e8 52fe ffff 8d64  $@.|$...$.R....d
+000014a0: 242c 5b5e 5f5d c389 f68d bc27 0000 0000  $,[^_].....'....
+000014b0: 53e8 95fc ffff 81c3 9e3a 0000 8d64 24e8  S........:...d$.
+000014c0: 8b44 2424 c744 2408 0000 0000 c704 240c  .D$$.D$.......$.
+000014d0: 0000 0089 4424 0c8b 4424 2089 4424 04e8  ....D$..D$ .D$..
+000014e0: 8cf4 ffff 85c0 7808 31c0 8d64 2418 5bc3  ......x.1..d$.[.
+000014f0: 8d83 dce1 ffff 8904 24e8 a2f4 ffff b8ff  ........$.......
+00001500: ffff ffeb e58d 7426 008d bc27 0000 0000  ......t&...'....
+00001510: 53e8 35fc ffff 81c3 3e3a 0000 8d64 24e8  S.5.....>:...d$.
+00001520: 8b44 2424 c744 2408 0000 0000 c704 240d  .D$$.D$.......$.
+00001530: 0000 0089 4424 0c8b 4424 2089 4424 04e8  ....D$..D$ .D$..
+00001540: 2cf4 ffff 85c0 7808 31c0 8d64 2418 5bc3  ,.....x.1..d$.[.
+00001550: 8d83 08e2 ffff 8904 24e8 42f4 ffff b8ff  ........$.B.....
+00001560: ffff ffeb e58d 7426 008d bc27 0000 0000  ......t&...'....
+00001570: 5557 568d 6424 a08b 7c24 708d 6c24 1c89  UWV.d$..|$p.l$..
+00001580: 6c24 0489 3c24 e825 ffff ff8b 7424 5889  l$..<$.%....t$X.
+00001590: 6c24 0489 3c24 2b74 2478 83e6 fc89 7424  l$..<$+t$x....t$
+000015a0: 58e8 6aff ffff 8b44 2478 8974 2404 893c  X.j....D$x.t$..<
+000015b0: 2489 4424 0c8b 4424 7489 4424 08e8 2efd  $.D$..D$t.D$....
+000015c0: ffff 8d64 2460 89f0 5e5f 5dc3 8d74 2600  ...d$`..^_]..t&.
+000015d0: 53e8 75fb ffff 81c3 7e39 0000 8d64 24e8  S.u.....~9...d$.
+000015e0: 8b44 2420 c744 240c 0000 0000 c744 2408  .D$ .D$......D$.
+000015f0: 0000 0000 c704 2407 0000 0089 4424 04e8  ......$.....D$..
+00001600: 6cf3 ffff 85c0 7808 31c0 8d64 2418 5bc3  l.....x.1..d$.[.
+00001610: 8d83 4ade ffff 8904 24e8 82f3 ffff b8ff  ..J.....$.......
+00001620: ffff ffeb e58d 7426 008d bc27 0000 0000  ......t&...'....
+00001630: 5531 ed57 5653 e810 fbff ff81 c319 3900  U1.WVS........9.
+00001640: 008d 6424 c48d bb56 deff ff8b 4424 5c89  ..d$...V....D$\.
+00001650: 3c24 8b74 2450 8944 2408 8b44 2454 8944  <$.t$P.D$..D$T.D
+00001660: 2404 e8e9 f2ff ff8b 4424 5c89 7c24 08c7  $.......D$\.|$..
+00001670: 0424 0300 0000 8944 2410 8b44 2454 8944  .$.....D$..D$T.D
+00001680: 240c 8d83 26de ffff 8944 2404 e8cf f2ff  $...&....D$.....
+00001690: ff8b 5424 5c8b 4424 5885 d28d 7c90 fc74  ..T$\.D$X...|..t
+000016a0: 2feb 0d90 9090 9090 9090 9090 9090 9090  /...............
+000016b0: 897c 2404 83c5 01c7 4424 0804 0000 0083  .|$.....D$......
+000016c0: ef04 8934 24e8 a6fe ffff 3b6c 245c 75e0  ...4$.....;l$\u.
+000016d0: c744 2408 0400 0000 8d44 242c 8934 2489  .D$......D$,.4$.
+000016e0: 4424 04c7 4424 2c40 4141 41e8 80fe ffff  D$..D$,@AAA.....
+000016f0: 8b44 2460 8934 2489 4424 04e8 b0fd ffff  .D$`.4$.D$......
+00001700: 8b44 2460 8b4c 2454 8948 3089 4424 0489  .D$`.L$T.H0.D$..
+00001710: 3424 e8f9 fdff ff83 f8ff 744c 8934 24e8  4$........tL.4$.
+00001720: acfe ffff 83f8 ff74 3f89 3424 c744 2408  .......t?.4$.D$.
+00001730: 0200 0000 c744 2404 0000 0000 e86f f2ff  .....D$......o..
+00001740: ff8b 4424 6089 3424 8944 2404 e85f fdff  ..D$`.4$.D$.._..
+00001750: ff8b 4424 608b 4018 8d64 243c 5b5e 5f5d  ..D$`.@..d$<[^_]
+00001760: c38d b426 0000 0000 8d64 243c b8ff ffff  ...&.....d$<....
+00001770: ff5b 5e5f 5dc3 8d76 008d bc27 0000 0000  .[^_]..v...'....
+00001780: 53e8 c5f9 ffff 81c3 ce37 0000 8d64 24e8  S........7...d$.
+00001790: 8b44 2420 c744 240c 0000 0000 c744 2408  .D$ .D$......D$.
+000017a0: 0000 0000 c704 2411 0000 0089 4424 04e8  ......$.....D$..
+000017b0: bcf1 ffff 85c0 7808 31c0 8d64 2418 5bc3  ......x.1..d$.[.
+000017c0: 8d83 71de ffff 8904 24e8 d2f1 ffff b8ff  ..q.....$.......
+000017d0: ffff ffeb e58d 7426 008d bc27 0000 0000  ......t&...'....
+000017e0: 5557 5653 e862 f9ff ff81 c36b 3700 008d  UWVS.b.....k7...
+000017f0: 6424 d48d ab9c deff ff8b 7424 40c7 4424  d$........t$@.D$
+00001800: 1c14 0000 00c7 4424 1800 0000 00c7 4424  ......D$......D$
+00001810: 0c00 0000 00c7 4424 0800 0000 0089 7424  ......D$......t$
+00001820: 04c7 0424 1000 0000 e843 f1ff ff85 c00f  ...$.....C......
+00001830: 88a3 0100 00c7 4424 0802 0000 00c7 4424  ......D$......D$
+00001840: 0400 0000 0089 3424 e863 f1ff ffc7 4424  ......4$.c....D$
+00001850: 0c00 0000 00c7 4424 0800 0000 0089 7424  ......D$......t$
+00001860: 04c7 0424 1800 0000 e803 f1ff ff85 c00f  ...$............
+00001870: 8843 0100 00c7 4424 0802 0000 00c7 4424  .C....D$......D$
+00001880: 0400 0000 0089 3424 e823 f1ff ffc7 4424  ......4$.#....D$
+00001890: 0c00 0000 00c7 4424 082c 0000 0089 7424  ......D$.,....t$
+000018a0: 04c7 0424 0300 0000 e8c3 f0ff ff89 4424  ...$..........D$
+000018b0: 0489 c789 2c24 e895 f0ff ff89 7c24 0c8d  ....,$......|$..
+000018c0: 8326 deff ff89 6c24 08c7 0424 0300 0000  .&....l$...$....
+000018d0: 8944 2404 8944 2414 e883 f0ff ffc7 4424  .D$..D$.......D$
+000018e0: 0c00 0000 00c7 4424 0800 0000 0089 7424  ......D$......t$
+000018f0: 04c7 0424 1800 0000 e873 f0ff ff85 c00f  ...$.....s......
+00001900: 88b3 0000 00c7 4424 0802 0000 00c7 4424  ......D$......D$
+00001910: 0400 0000 0089 3424 e893 f0ff ffc7 4424  ......4$......D$
+00001920: 0c00 0000 00c7 4424 082c 0000 0089 7424  ......D$.,....t$
+00001930: 04c7 0424 0300 0000 e833 f0ff ff89 4424  ...$.....3....D$
+00001940: 0489 c789 2c24 e805 f0ff ff8b 4424 1489  ....,$......D$..
+00001950: 7c24 0c89 6c24 08c7 0424 0300 0000 8944  |$..l$...$.....D
+00001960: 2404 e8f9 efff ff8b 4424 4485 c074 2139  $.......D$D..t!9
+00001970: bb0c 0100 0074 2189 3424 e801 feff ff83  .....t!.4$......
+00001980: 6c24 1c01 744a 897c 2418 e97e feff ff90  l$..tJ.|$..~....
+00001990: 39bb 0c01 0000 750e 8b44 2418 2df0 0000  9.....u..D$.-...
+000019a0: 0083 f801 76d1 31c0 8d64 242c 5b5e 5f5d  ....v.1..d$,[^_]
+000019b0: c38d b426 0000 0000 8d83 8dde ffff 8904  ...&............
+000019c0: 24e8 daef ffff b8ff ffff ffeb db8d 7600  $.............v.
+000019d0: b8ff ffff ffeb d190 8d83 7fde ffff 8904  ................
+000019e0: 24e8 baef ffff b8ff ffff ffeb bb8d 7600  $.............v.
+000019f0: 5557 5653 e852 f7ff ff81 c35b 3500 008d  UWVS.R.....[5...
+00001a00: a424 b4fb ffff 8b8b f0ff ffff 8b84 2460  .$............$`
+00001a10: 0400 008b ac24 6404 0000 8b11 85c0 8994  .....$d.........
+00001a20: 243c 0400 000f 88d5 0000 0089 4424 0c8d  $<..........D$..
+00001a30: 7424 1cc7 4424 0420 0000 008d 83b5 deff  t$..D$. ........
+00001a40: ff89 3424 8944 2408 e873 efff ff89 3424  ..4$.D$..s....4$
+00001a50: 8d83 c3de ffff 8944 2404 8d74 243c e86d  .......D$..t$<.m
+00001a60: efff ff85 c089 c775 17e9 bb00 0000 6690  .......u......f.
+00001a70: 896c 2404 8934 24e8 64ef ffff 85c0 7548  .l$..4$.d.....uH
+00001a80: 897c 2408 c744 2404 0004 0000 8934 24e8  .|$..D$......4$.
+00001a90: 5cef ffff 85c0 75d8 31f6 893c 24e8 5eef  \.....u.1..<$.^.
+00001aa0: ffff 8b93 f0ff ffff 89f0 8b8c 243c 0400  ............$<..
+00001ab0: 008b 1239 d175 798d a424 4c04 0000 5b5e  ...9.uy..$L...[^
+00001ac0: 5f5d c390 8d74 2600 8934 248d 83c5 deff  _]...t&..4$.....
+00001ad0: ff89 4424 04e8 36ef ffff 8904 24c7 4424  ..D$..6.....$.D$
+00001ae0: 0810 0000 00c7 4424 0400 0000 00e8 2eef  ......D$........
+00001af0: ffff 3d00 8000 0089 c675 9feb 9b8d 7600  ..=......u....v.
+00001b00: c744 241c 2f70 726f 8d74 241c c744 2420  .D$./pro.t$..D$ 
+00001b10: 632f 7365 c744 2424 6c66 2f6d c744 2428  c/se.D$$lf/m.D$(
+00001b20: 6170 7300 e924 ffff ff31 f6e9 72ff ffff  aps..$...1..r...
+00001b30: e8fb f5ff ff8d 7426 008d bc27 0000 0000  ......t&...'....
+00001b40: 5756 8d64 24ec 8b74 2424 c704 24ff ffff  WV.d$..t$$..$...
+00001b50: ff89 7424 04e8 96fe ffff 8974 2404 89c7  ..t$.......t$...
+00001b60: 8b44 2420 8904 24e8 84fe ffff 0344 2428  .D$ ..$......D$(
+00001b70: 8d64 2414 5e29 f85f c38d b426 0000 0000  .d$.^)._...&....
+00001b80: 5557 5653 e8c2 f5ff ff81 c3cb 3300 008d  UWVS........3...
+00001b90: a424 64ff ffff 8bbc 24b0 0000 00c7 4424  .$d.....$.....D$
+00001ba0: 0400 0000 0089 3c24 e883 eeff ff83 f8ff  ......<$........
+00001bb0: 89c6 0f84 3702 0000 8934 248d 4424 3089  ....7....4$.D$0.
+00001bc0: 4424 04e8 78ee ffff 8b7c 245c 893c 24e8  D$..x....|$\.<$.
+00001bd0: 7cee ffff 8904 2489 c589 7c24 08c7 4424  |.....$...|$..D$
+00001be0: 0400 0000 0089 4424 24e8 72ee ffff 897c  ......D$$.r....|
+00001bf0: 2408 896c 2404 8934 24e8 72ee ffff 8934  $..l$..4$.r....4
+00001c00: 24e8 7aee ffff 8b4d 200f b77d 2e01 e985  $.z....M ..}....
+00001c10: ff0f 8421 0200 008b 4104 31f6 c744 2420  ...!....A.1..D$ 
+00001c20: 0000 0000 c744 2428 0000 0000 c744 242c  .....D$(.....D$,
+00001c30: 0000 0000 c744 241c 0000 0000 eb37 6690  .....D$......7f.
+00001c40: 8b41 1031 d289 4424 208b 4114 f771 2489  .A.1..D$ .A..q$.
+00001c50: 4424 1c89 e884 c00f 85fb 0000 0083 c601  D$..............
+00001c60: 39fe 7d4c 8b69 288b 412c 85ed 7504 85c0  9.}L.i(.A,..u...
+00001c70: 743e 83c1 2883 f80b 0f94 c289 d574 c183  t>..(........t..
+00001c80: f802 74bc 83f8 0375 d48b 4424 240f b740  ..t....u..D$$..@
+00001c90: 3239 f074 c88b 4110 83c6 0139 fe89 4424  29.t..A....9..D$
+00001ca0: 287c c18d b600 0000 008d bc27 0000 0000  (|.........'....
+00001cb0: 8b4c 2420 8b44 2428 85c9 0f84 dd00 0000  .L$ .D$(........
+00001cc0: 8b54 241c 85d2 0f84 d100 0000 8b54 2428  .T$..........T$(
+00001cd0: 85d2 0f84 c900 0000 8b44 2424 8b7c 2420  .........D$$.|$ 
+00001ce0: 8b74 2428 01c7 01c6 8b44 241c 85c0 0f8e  .t$(.....D$.....
+00001cf0: 2a01 0000 31ed 89f8 89ef 89c5 eb12 6690  *...1.........f.
+00001d00: 83c7 0183 c510 3b7c 241c 0f84 0e01 0000  ......;|$.......
+00001d10: 8b84 24b4 0000 0089 4424 048b 4500 01f0  ..$.....D$..E...
+00001d20: 8904 24e8 68ed ffff 85c0 75d4 8b44 2424  ..$.h.....u..D$$
+00001d30: 8b75 0489 0424 e865 edff ff85 f60f 84e7  .u...$.e........
+00001d40: 0000 0089 f02b 4424 2c8d a424 9c00 0000  .....+D$,..$....
+00001d50: 5b5e 5f5d c38d 7600 8b54 2424 8b42 1c0f  [^_]..v..T$$.B..
+00001d60: b76a 2c01 d066 85ed 0f84 effe ffff 83c5  .j,..f..........
+00001d70: 01ba 0100 0000 eb0e 83c2 0183 c020 39ea  ............. 9.
+00001d80: 0f84 d7fe ffff 8338 0175 ed83 7804 0075  .......8.u..x..u
+00001d90: e78b 4008 8944 242c e9c0 feff ff8b 4424  ..@..D$,......D$
+00001da0: 2889 4424 148b 4424 1cc7 0424 0600 0000  (.D$..D$...$....
+00001db0: 8944 2410 8b44 2420 8944 240c 8d83 34e2  .D$..D$ .D$...4.
+00001dc0: ffff 8944 2408 8d83 26de ffff 8944 2404  ...D$...&....D$.
+00001dd0: e88b ebff ff8b 4424 2489 0424 e8bf ecff  ......D$$..$....
+00001de0: ff8d a424 9c00 0000 31c0 5b5e 5f5d c389  ...$....1.[^_]..
+00001df0: 7c24 088d 83c7 deff ff89 4424 048b 83f4  |$........D$....
+00001e00: ffff ff05 a800 0000 8904 24e8 a0ec ffff  ..........$.....
+00001e10: 8da4 249c 0000 0031 c05b 5e5f 5dc3 8b44  ..$....1.[^_]..D
+00001e20: 2424 8904 24e8 76ec ffff 8da4 249c 0000  $$..$.v.....$...
+00001e30: 0031 c05b 5e5f 5dc3 c744 241c 0000 0000  .1.[^_]..D$.....
+00001e40: 31c0 c744 2420 0000 0000 e952 ffff ff90  1..D$ .....R....
+00001e50: 5557 5653 e8f2 f2ff ff81 c3fb 3000 008d  UWVS........0...
+00001e60: 6424 d48d abd8 deff ff8b 7c24 40e8 def2  d$........|$@...
+00001e70: ffff 8944 2404 89c6 892c 24e8 d0ea ffff  ...D$....,$.....
+00001e80: 896c 2408 8dab 26de ffff 8974 240c c704  .l$...&....t$...
+00001e90: 2403 0000 0089 6c24 04e8 c2ea ffff 83fe  $.....l$........
+00001ea0: 1c7e 1689 3c24 8d83 2c02 0000 8944 2404  .~..<$..,....D$.
+00001eb0: e8db ebff ff85 c074 2fc7 4424 0400 0000  .......t/.D$....
+00001ec0: 0089 3c24 e8f7 ebff ff8b 4c24 4489 0424  ..<$......L$D..$
+00001ed0: 894c 2404 e8f7 ebff ff85 c074 0b8d 6424  .L$........t..d$
+00001ee0: 2c5b 5e5f 5dc3 6690 8b44 2444 893c 2489  ,[^_].f..D$D.<$.
+00001ef0: 4424 04e8 88fc ffff 8d93 edde ffff 89c6  D$..............
+00001f00: 8944 2404 8914 2489 5424 1ce8 40ea ffff  .D$...$.T$..@...
+00001f10: 8b54 241c 8974 240c 896c 2404 c704 2403  .T$..t$..l$...$.
+00001f20: 0000 0089 5424 08e8 34ea ffff 31c0 85f6  ....T$..4...1...
+00001f30: 74ab 897c 2404 c704 24ff ffff ffe8 aefa  t..|$...$.......
+00001f40: ffff 8d64 242c 01f0 5b5e 5f5d c38d 7600  ...d$,..[^_]..v.
+00001f50: 5557 5653 e8f2 f1ff ff81 c3fb 2f00 008d  UWVS......../...
+00001f60: a424 a4fe ffff 8b83 f0ff ffff 8bbc 2470  .$............$p
+00001f70: 0100 008b 0085 ff89 8424 4c01 0000 0f84  .........$L.....
+00001f80: f400 0000 8d83 f7de ffff 8904 24e8 4eeb  ............$.N.
+00001f90: ffff 85c0 89c6 0f84 dc00 0000 8d83 fdde  ................
+00001fa0: ffff 8944 2414 eb11 83c0 1389 0424 e88d  ...D$........$..
+00001fb0: e9ff ff85 c089 c575 3f89 3424 e82f ebff  .......u?.4$./..
+00001fc0: ff85 c075 e3bd ffff ffff 8934 24e8 2eeb  ...u.......4$...
+00001fd0: ffff 89e8 8bbb f0ff ffff 8b8c 244c 0100  ............$L..
+00001fe0: 008b 1739 d10f 859a 0000 008d a424 5c01  ...9.........$\.
+00001ff0: 0000 5b5e 5f5d c390 8944 2408 8d54 242c  ..[^_]...D$..T$,
+00002000: 8b44 2414 8914 2489 5424 1889 4424 04e8  .D$...$.T$..D$..
+00002010: fcea ffff 8b54 2418 8d83 c3de ffff 8944  .....T$........D
+00002020: 2404 8914 24e8 a6e9 ffff 85c0 748b 8944  $...$.......t..D
+00002030: 2408 8d4c 244c c744 2404 0001 0000 890c  $..L$L.D$.......
+00002040: 2489 4424 1c89 4c24 18e8 a2e9 ffff 8b54  $.D$..L$.......T
+00002050: 241c 8914 24e8 a6e9 ffff 8b4c 2418 893c  $...$......L$..<
+00002060: 2489 4c24 04e8 26ea ffff 85c0 0f85 47ff  $.L$..&.......G.
+00002070: ffff e953 ffff ff90 b8ff ffff ff8d 7600  ...S..........v.
+00002080: e94f ffff ffe8 a6f0 ffff 8db6 0000 0000  .O..............
+00002090: 5557 5653 e8b2 f0ff ff81 c3bb 2e00 008d  UWVS............
+000020a0: 6424 a48d bb2c 0300 008d 830e dfff ff8d  d$...,..........
+000020b0: b313 dfff ff89 3c24 8944 2404 e88f fdff  ......<$.D$.....
+000020c0: ff89 4424 0889 4424 1c8b 4424 7089 7c24  ..D$..D$..D$p.|$
+000020d0: 0489 0424 e867 faff ff89 3424 89c5 8b44  ...$.g....4$...D
+000020e0: 2474 8944 2404 e865 e8ff ff8b 4424 7489  $t.D$..e....D$t.
+000020f0: 7424 088d b326 deff ffc7 0424 0300 0000  t$...&.....$....
+00002100: 8944 240c 8974 2404 e853 e8ff ff89 7c24  .D$..t$..S....|$
+00002110: 048d 8b2d dfff ff89 0c24 894c 2418 e82d  ...-.....$.L$..-
+00002120: e8ff ff8b 4c24 1889 7c24 0c8d bb40 dfff  ....L$..|$...@..
+00002130: ff89 7424 04c7 0424 0300 0000 894c 2408  ..t$...$.....L$.
+00002140: e81b e8ff ff8b 5424 1c89 3c24 8954 2404  ......T$..<$.T$.
+00002150: 8954 2418 e8f7 e7ff ff8b 5424 1889 7c24  .T$.......T$..|$
+00002160: 088d bb59 dfff ff89 7424 04c7 0424 0300  ...Y....t$...$..
+00002170: 0000 8954 240c e8e5 e7ff ff89 6c24 0489  ...T$.......l$..
+00002180: 3c24 e8c9 e7ff ff89 6c24 0c89 7c24 088d  <$......l$..|$..
+00002190: bb70 e2ff ff89 7424 04c7 0424 0300 0000  .p....t$...$....
+000021a0: e8bb e7ff ff8b 4424 7489 3c24 c744 2428  ......D$t.<$.D$(
+000021b0: 0000 0000 8944 242c 8b44 2470 c744 2430  .....D$,.D$p.D$0
+000021c0: 0300 0000 c744 2434 2200 0000 8944 2404  .....D$4"....D$.
+000021d0: c744 2438 0000 0000 c744 243c 0000 0000  .D$8.....D$<....
+000021e0: e86b e7ff ff8b 4424 7089 7c24 0889 7424  .k....D$p.|$..t$
+000021f0: 04c7 0424 0300 0000 8944 240c e85f e7ff  ...$.....D$.._..
+00002200: ff8b 4424 7889 6c24 048d ab73 dfff ffc7  ..D$x.l$...s....
+00002210: 4424 0c06 0000 0089 4424 108d 4424 2889  D$......D$..D$(.
+00002220: 4424 088b 4424 7089 0424 e801 f4ff ff89  D$..D$p..$......
+00002230: 4424 0489 c789 2c24 e813 e7ff ff89 7c24  D$....,$......|$
+00002240: 0c89 6c24 0889 7424 04c7 0424 0300 0000  ..l$..t$...$....
+00002250: e80b e7ff ff8d 6424 5c89 f85b 5e5f 5dc3  ......d$\..[^_].
+00002260: 5557 5653 e8e2 eeff ff81 c3eb 2c00 008d  UWVS........,...
+00002270: 6424 848d bb2c 0300 0089 3c24 8d6c 242c  d$...,....<$.l$,
+00002280: c744 2404 0000 0000 8bb4 2490 0000 00e8  .D$.......$.....
+00002290: 2ce8 ffff 8904 248d 938d dfff ff89 5424  ,.....$.......T$
+000022a0: 04e8 2ae8 ffff 8944 2408 897c 2404 8934  ..*....D$..|$..4
+000022b0: 24e8 8af8 ffff 896c 2404 89c7 8934 24e8  $......l$....4$.
+000022c0: ecf1 ffff 83f8 ff74 7a89 6c24 108d ab95  .......tz.l$....
+000022d0: dfff ff89 7c24 04c7 4424 0c00 0000 00c7  ....|$..D$......
+000022e0: 4424 0800 0000 0089 3424 e841 f3ff ff89  D$......4$.A....
+000022f0: 4424 0489 c789 2c24 c744 2428 0000 0000  D$....,$.D$(....
+00002300: e84b e6ff ff89 7c24 0c8d 8326 deff ff89  .K....|$...&....
+00002310: 6c24 08c7 0424 0300 0000 8944 2404 e83d  l$...$.....D$..=
+00002320: e6ff ffc7 4424 0c04 0000 008d 4424 2889  ....D$......D$(.
+00002330: 7c24 0489 3424 8944 2408 e8d1 eeff ff8b  |$..4$.D$.......
+00002340: 4424 288d 6424 7c5b 5e5f 5dc3 8d74 2600  D$(.d$|[^_]..t&.
+00002350: 5557 5653 e8f2 edff ff81 c3fb 2b00 008d  UWVS........+...
+00002360: 6424 d48b 4424 4c8b 7424 488b 7c24 5089  d$..D$L.t$H.|$P.
+00002370: 4424 088b 4424 4089 7424 0489 7c24 0c89  D$..D$@.t$..|$..
+00002380: 0424 e889 eeff ff85 c00f 88b1 0000 0089  .$..............
+00002390: fd83 ed01 0f88 9e00 0000 8b44 244c 8b54  ...........D$L.T
+000023a0: 2444 0fb6 4438 ff38 443a ff74 6b89 6c24  $D..D8.8D:.tk.l$
+000023b0: 088d bb98 e2ff ff89 7424 0489 3c24 e88d  ........t$..<$..
+000023c0: e5ff ff89 7c24 088d 8326 deff ff89 6c24  ....|$...&....l$
+000023d0: 108d 7d01 8974 240c c704 2403 0000 0089  ..}..t$...$.....
+000023e0: 4424 04e8 78e5 ffff 8b44 2444 897c 240c  D$..x....D$D.|$.
+000023f0: 8974 2404 8944 2408 8b44 2440 8904 24e8  .t$..D$..D$@..$.
+00002400: ecee ffff 85c0 7838 8d64 242c 89f8 5b5e  ......x8.d$,..[^
+00002410: 5f5d c390 8d74 2600 83ed 0183 fdff 7418  _]...t&.......t.
+00002420: 8b44 244c 8b4c 2444 0fb6 0428 3804 290f  .D$L.L$D...(8.).
+00002430: 8578 ffff ffeb e190 31ff ebcc 8d74 2600  .x......1....t&.
+00002440: bfff ffff ffeb c189 f68d bc27 0000 0000  ...........'....
+00002450: 55b9 4000 0000 5756 53e8 edec ffff 81c3  U.@...WVS.......
+00002460: f62a 0000 8da4 24c4 feff ff8b 8424 5c01  .*....$......$\.
+00002470: 0000 8d7c 242c 8bb4 2458 0100 008b ac24  ...|$,..$X.....$
+00002480: 6401 0000 8944 2418 8b83 f0ff ffff 8b00  d....D$.........
+00002490: 8984 242c 0100 0031 c0f3 ab8b 8424 5401  ..$,...1.....$T.
+000024a0: 0000 8d7c 242c c744 2410 1000 0000 8974  ...|$,.D$......t
+000024b0: 2408 8944 2404 8b84 2450 0100 0089 7c24  $..D$...$P....|$
+000024c0: 0c89 0424 e887 feff ff85 c00f 887f 0000  ...$............
+000024d0: 0089 4424 1c8b 8424 6001 0000 896c 2410  ..D$...$`....l$.
+000024e0: 8974 2404 8944 240c 8b44 2418 8944 2408  .t$..D$..D$..D$.
+000024f0: 8b84 2450 0100 0089 0424 e831 f1ff ff8b  ..$P.....$.1....
+00002500: 5424 1c89 c585 d274 258b 8424 5001 0000  T$.....t%..$P...
+00002510: 8954 240c 897c 2408 8974 2404 8904 24e8  .T$..|$..t$...$.
+00002520: cced ffff 85c0 b8ff ffff ff0f 48e8 8bb3  ............H...
+00002530: f0ff ffff 89e8 8b8c 242c 0100 008b 1639  ........$,.....9
+00002540: d175 358d a424 3c01 0000 5b5e 5f5d c390  .u5..$<...[^_]..
+00002550: 8944 2408 8d83 badf ffff 8944 2404 bdff  .D$........D$...
+00002560: ffff ff8b 83f4 ffff ff05 a800 0000 8904  ................
+00002570: 24e8 3ae5 ffff ebb6 e8b3 ebff ff8d 7600  $.:...........v.
+00002580: 5557 5653 e8c2 ebff ff81 c3cb 2900 008d  UWVS........)...
+00002590: a424 14ff ffff 8db3 ccdf ffff 8bac 2400  .$............$.
+000025a0: 0100 0089 3424 896c 2404 e8a1 e3ff ff89  ....4$.l$.......
+000025b0: 7424 088d 8326 deff ff89 6c24 0cc7 0424  t$...&....l$...$
+000025c0: 0300 0000 8944 2404 8944 2418 e88f e3ff  .....D$..D$.....
+000025d0: ff8b 8424 1401 0000 892c 2489 4424 04e8  ...$.....,$.D$..
+000025e0: fcf1 ffff 83f8 ff89 c60f 8427 0200 0089  ...........'....
+000025f0: 2c24 8d44 2458 8944 2404 8944 241c e8ad  ,$.D$X.D$..D$...
+00002600: eeff ff83 f8ff 89c6 0f84 0002 0000 8b74  ...............t
+00002610: 241c 8dbc 249c 0000 0089 7c24 20b9 1100  $...$.....|$ ...
+00002620: 0000 f3a5 e827 ebff ff8b 7424 1c89 c7c7  .....'....t$....
+00002630: 4424 0400 1000 0089 2c24 8974 2408 e84d  D$......,$.t$..M
+00002640: faff ff83 f8ff 89c6 0f84 3a05 0000 83ff  ..........:.....
+00002650: 190f 8fc9 0300 008b 83f8 ffff ff89 2c24  ..............,$
+00002660: 8944 2408 8d83 2c02 0000 8944 2404 e8cd  .D$...,....D$...
+00002670: f4ff ff89 c78d 932c 0100 0089 1424 8d83  .......,.....$..
+00002680: 89e0 ffff 8944 2404 8954 2424 e8bf f7ff  .....D$..T$$....
+00002690: ff8b 5424 2489 4424 0889 2c24 8954 2404  ..T$$.D$..,$.T$.
+000026a0: e89b f4ff ff89 4424 088d 93d0 e3ff ff89  ......D$........
+000026b0: 7c24 0489 1424 8944 2428 8954 2424 e88d  |$...$.D$(.T$$..
+000026c0: e2ff ff8b 5424 248b 4c24 288b 4424 1889  ....T$$.L$(.D$..
+000026d0: 7c24 0c89 5424 0889 4c24 10c7 0424 0300  |$..T$..L$...$..
+000026e0: 0000 8944 2404 e875 e2ff ff8b 8c24 0401  ...D$..u.....$..
+000026f0: 0000 8974 2404 892c 2489 4c24 08e8 0eed  ...t$..,$.L$....
+00002700: ffff 8b8c 2404 0100 008d 93e8 e2ff ff89  ....$...........
+00002710: 1424 8974 2430 894c 2404 c744 2434 0200  .$.t$0.L$..D$4..
+00002720: 0000 8954 2424 e825 e2ff ff8b 8c24 0401  ...T$$.%.....$..
+00002730: 0000 8b54 2424 8b44 2418 c704 2403 0000  ...T$$.D$...$...
+00002740: 0089 4c24 0c89 5424 0889 4424 04e8 0ee2  ..L$..T$..D$....
+00002750: ffff 8b8b f8ff ffff b802 0000 008b 5424  ..............T$
+00002760: 1c89 4424 108d 4424 3089 4c24 0489 7c24  ..D$..D$0.L$..|$
+00002770: 0889 5424 1489 2c24 8944 240c 8944 2424  ..T$..,$.D$..D$$
+00002780: e8cb fcff ff8d 9314 e3ff ff89 c789 4424  ..............D$
+00002790: 0489 1424 8954 2428 e8b3 e1ff ff8b 5424  ...$.T$(......T$
+000027a0: 288b 4424 1889 7c24 0c83 ef01 c704 2403  (.D$..|$......$.
+000027b0: 0000 0089 5424 0889 4424 04e8 a0e1 ffff  ....T$..D$......
+000027c0: 83ff fd76 6389 2c24 e893 faff ff89 4424  ...vc.,$......D$
+000027d0: 0c8b 8424 0401 0000 8944 2408 8d83 3fe0  ...$.....D$...?.
+000027e0: ffff 8944 2404 beff ffff ff8b 83f4 ffff  ...D$...........
+000027f0: ff05 a800 0000 8904 24e8 b2e2 ffff 8b44  ........$......D
+00002800: 2420 892c 2489 4424 04e8 02ed ffff 892c  $ .,$.D$.......,
+00002810: 24e8 6aef ffff 8da4 24ec 0000 0089 f05b  $.j.....$......[
+00002820: 5e5f 5dc3 8d74 2600 8b84 2408 0100 0089  ^_]..t&...$.....
+00002830: 4424 048b 8424 0401 0000 8904 24e8 3ef3  D$...$......$.>.
+00002840: ffff 89c7 8b84 2404 0100 0085 ff0f 8415  ......$.........
+00002850: 0300 0089 4424 0489 2c24 e891 f1ff ff89  ....D$..,$......
+00002860: 4424 088d 8b34 e3ff ff89 4424 288b 8424  D$...4....D$(..$
+00002870: 0401 0000 890c 2489 4c24 2c89 4424 04e8  ......$.L$,.D$..
+00002880: cce0 ffff 8b84 2404 0100 008b 5424 288b  ......$.....T$(.
+00002890: 4c24 2c89 4424 0c8b 4424 1889 5424 10c7  L$,.D$..D$..T$..
+000028a0: 0424 0300 0000 894c 2408 8944 2404 e8ad  .$.....L$..D$...
+000028b0: e0ff ff8b 5424 2885 d20f 8401 0300 008b  ....T$(.........
+000028c0: 8c24 0801 0000 8d04 3a89 4424 088d bb54  .$......:.D$...T
+000028d0: e3ff ff89 3c24 894c 2404 8944 2428 e86d  ....<$.L$..D$(.m
+000028e0: e0ff ff8b 4424 2889 7c24 0831 ffc7 0424  ....D$(.|$.1...$
+000028f0: 0300 0000 8944 2410 8b84 2408 0100 0089  .....D$...$.....
+00002900: 4424 0c8b 4424 1889 4424 04e8 50e0 ffff  D$..D$..D$..P...
+00002910: 8b94 2410 0100 0031 c085 d274 6389 ac24  ..$....1...tc..$
+00002920: 0001 0000 8db6 0000 0000 8dbf 0000 0000  ................
+00002930: 8b8c 240c 0100 008d 2c81 8b45 0089 7424  ..$.....,..E..t$
+00002940: 0489 4424 088b 8424 0001 0000 8904 24e8  ..D$...$......$.
+00002950: bcea ffff 8b44 2424 8934 b883 c701 8b45  .....D$$.4.....E
+00002960: 0089 0424 e827 e0ff ff01 c689 f883 c601  ...$.'..........
+00002970: 3bbc 2410 0100 0075 b78b ac24 0001 0000  ;.$....u...$....
+00002980: 8b84 2408 0100 008d b378 e3ff ff89 3424  ..$......x....4$
+00002990: 8dbb a4e3 ffff 8944 2404 e8b1 dfff ff8b  .......D$.......
+000029a0: 8424 0801 0000 8974 2408 c704 2403 0000  .$.....t$...$...
+000029b0: 0089 4424 0c8b 4424 1889 4424 04e8 9edf  ..D$..D$..D$....
+000029c0: ffff 8b4c 241c 892c 2489 4c24 108b 8c24  ...L$..,$.L$...$
+000029d0: 1001 0000 894c 240c 8b4c 2424 894c 2408  .....L$..L$$.L$.
+000029e0: 8b4c 2428 894c 2404 e843 ecff ff89 4424  .L$(.L$..C....D$
+000029f0: 0489 c689 3c24 e855 dfff ff8b 4424 1889  ....<$.U....D$..
+00002a00: 7424 0c89 7c24 08c7 0424 0300 0000 8944  t$..|$...$.....D
+00002a10: 2404 e849 dfff ffe9 e2fd ffff 8d74 2600  $..I.........t&.
+00002a20: 8d83 e7df ffff 8dbb 2c02 0000 8944 2404  ........,....D$.
+00002a30: 893c 24e8 18f4 ffff 85c0 89c1 0f84 b001  .<$.............
+00002a40: 0000 894c 2408 897c 2404 892c 2489 4c24  ...L$..|$..,$.L$
+00002a50: 2ce8 eaf0 ffff 89c7 8d93 2c01 0000 8914  ,.........,.....
+00002a60: 248d 8389 e0ff ff89 4424 0489 5424 24e8  $.......D$..T$$.
+00002a70: dcf3 ffff 8b54 2424 8944 2408 892c 2489  .....T$$.D$..,$.
+00002a80: 5424 04e8 b8f0 ffff 8944 2408 8d93 d0e3  T$.......D$.....
+00002a90: ffff 897c 2404 8914 2489 4424 2489 5424  ...|$...$.D$$.T$
+00002aa0: 28e8 aade ffff 8b44 2424 8b54 2428 897c  (......D$$.T$(.|
+00002ab0: 240c 8944 2410 8b44 2418 c704 2403 0000  $..D$..D$...$...
+00002ac0: 0089 5424 0889 4424 04e8 92de ffff 8b84  ..T$..D$........
+00002ad0: 2404 0100 0089 7424 0489 2c24 8944 2408  $.....t$..,$.D$.
+00002ae0: e82b e9ff ff8b 4c24 2c8d 832c 0300 0089  .+....L$,..,....
+00002af0: 2c24 8944 2404 8974 2430 c744 2434 0200  ,$.D$..t$0.D$4..
+00002b00: 0000 894c 2428 e8e5 eeff ff89 4424 388d  ...L$(......D$8.
+00002b10: 93e8 e2ff ff8b 8424 0401 0000 8914 2489  .......$......$.
+00002b20: 5424 2489 4424 04e8 24de ffff 8b84 2404  T$$.D$..$.....$.
+00002b30: 0100 008b 5424 24c7 0424 0300 0000 8944  ....T$$..$.....D
+00002b40: 240c 8b44 2418 8954 2408 8944 2404 e80d  $..D$..T$..D$...
+00002b50: deff ff8b 4c24 28b8 0300 0000 e9fc fbff  ....L$(.........
+00002b60: ff8d b426 0000 0000 8944 240c 8b84 2408  ...&.....D$...$.
+00002b70: 0100 0089 4424 088d 8354 e0ff ffe9 60fc  ....D$...T....`.
+00002b80: ffff 8db6 0000 0000 8b83 f4ff ffff c744  ...............D
+00002b90: 2408 2600 0000 c744 2404 0100 0000 05a8  $.&....D$.......
+00002ba0: 0000 0089 4424 0c8d 83c0 e2ff ff89 0424  ....D$.........$
+00002bb0: e86b dfff ffe9 44fc ffff 8db6 0000 0000  .k....D.........
+00002bc0: 8b84 2404 0100 00be ffff ffff 8944 2408  ..$..........D$.
+00002bd0: 8d83 72e0 ffff 8944 2404 8b83 f4ff ffff  ..r....D$.......
+00002be0: 05a8 0000 0089 0424 e8c3 deff ffe9 0cfc  .......$........
+00002bf0: ffff 893c 248d 83fc dfff ff89 4424 04e8  ...<$.......D$..
+00002c00: 4cf2 ffff 85c0 89c1 0f85 34fe ffff 893c  L.........4....<
+00002c10: 248d 8314 e0ff ff89 4424 04e8 30f2 ffff  $.......D$..0...
+00002c20: 85c0 89c1 0f85 18fe ffff 8b83 f4ff ffff  ................
+00002c30: beff ffff ffc7 4424 081a 0000 00c7 4424  ......D$......D$
+00002c40: 0401 0000 0005 a800 0000 8944 240c 8d83  ...........D$...
+00002c50: 24e0 ffff 8904 24e8 c4de ffff e99d fbff  $.....$.........
+00002c60: ffeb 0d90 9090 9090 9090 9090 9090 9090  ................
+00002c70: 5756 53e8 d3e4 ffff 81c3 dc22 0000 8d64  WVS........"...d
+00002c80: 24f0 8b44 2428 8b7c 2424 8d70 ff8b 4424  $..D$(.|$$.p..D$
+00002c90: 2089 7c24 0489 7424 0889 0424 e88f deff   .|$..t$...$....
+00002ca0: ff85 c078 1339 c67e 0fc6 0407 008d 6424  ...x.9.~......d$
+00002cb0: 105b 5e5f c38d 7600 8d83 91e0 ffff 8904  .[^_..v.........
+00002cc0: 24e8 dadc ffff 8d64 2410 5b5e 5fc3 6690  $......d$.[^_.f.
+00002cd0: 5653 e874 e4ff ff81 c37d 2200 008d 6424  VS.t.....}"...d$
+00002ce0: 8c8b b424 8000 0000 8d44 2410 8944 2404  ...$.....D$..D$.
+00002cf0: 8934 24e8 48de ffff 8b44 2420 2500 f000  .4$.H....D$ %...
+00002d00: 003d 00a0 0000 7408 8d64 2474 5b5e c390  .=....t..d$t[^..
+00002d10: 8974 2404 8934 24c7 4424 0800 0100 00e8  .t$..4$.D$......
+00002d20: 4cff ffff 8d64 2474 5b5e c390 8d74 2600  L....d$t[^...t&.
+00002d30: 0800 0000 0400 0000 0100 0000 416e 6472  ............Andr
+00002d40: 6f69 6400 1500 0000 726f 2e62 7569 6c64  oid.....ro.build
+00002d50: 2e76 6572 7369 6f6e 2e73 646b 005b 2b5d  .version.sdk.[+]
+00002d60: 2041 6e64 726f 6964 2073 646b 2076 6572   Android sdk ver
+00002d70: 7369 6f6e 3a20 2564 0a00 696e 6a65 6374  sion: %d..inject
+00002d80: 005b 2b5d 2025 7020 7772 6974 6520 7374  .[+] %p write st
+00002d90: 7269 6e67 3a20 5b25 645d 2573 0a00 7074  ring: [%d]%s..pt
+00002da0: 7261 6365 5f63 6f6e 7400 5b2b 5d20 5838  race_cont.[+] X8
+00002db0: 3620 7074 7261 6365 2063 616c 6c20 2570  6 ptrace call %p
+00002dc0: 2025 640a 0070 7472 6163 655f 6465 7461   %d..ptrace_deta
+00002dd0: 6368 0070 7472 6163 655f 6174 7461 6368  ch.ptrace_attach
+00002de0: 0070 7472 6163 655f 7379 7363 616c 6c00  .ptrace_syscall.
+00002df0: 5b2b 5d20 4375 7272 656e 7420 7379 7363  [+] Current sysc
+00002e00: 616c 6c3a 2025 640a 002f 7072 6f63 2f25  all: %d../proc/%
+00002e10: 642f 6d61 7073 0072 002d 0043 616e 6e6f  d/maps.r.-.Canno
+00002e20: 7420 6f70 656e 2027 2573 2700 5b2b 5d20  t open '%s'.[+] 
+00002e30: 5344 4b20 7665 7273 696f 6e3a 2025 640a  SDK version: %d.
+00002e40: 0061 6464 723a 2025 640a 002f 7072 6f63  .addr: %d../proc
+00002e50: 002f 7072 6f63 2f25 642f 636d 646c 696e  ./proc/%d/cmdlin
+00002e60: 6500 6d6d 6170 005b 2b5d 2052 656d 6f74  e.mmap.[+] Remot
+00002e70: 6520 6d6d 6170 2025 6420 6279 7465 730a  e mmap %d bytes.
+00002e80: 005b 2b5d 206c 6962 635f 7061 7468 3a20  .[+] libc_path: 
+00002e90: 2570 0a00 5b2b 5d20 6c6f 6361 6c5f 6d6d  %p..[+] local_mm
+00002ea0: 6170 5f61 6464 723a 2025 700a 005b 2b5d  ap_addr: %p..[+]
+00002eb0: 2052 656d 6f74 6520 6d6d 6170 2061 6464   Remote mmap add
+00002ec0: 7220 2570 200a 005b 2b5d 2043 616c 6c20  r %p ..[+] Call 
+00002ed0: 6d6d 6170 2072 6573 756c 743a 2025 700a  mmap result: %p.
+00002ee0: 005f 5f65 7272 6e6f 005b 2b5d 2045 7272  .__errno.[+] Err
+00002ef0: 6e6f 2061 6464 723a 2025 700a 006d 6d61  no addr: %p..mma
+00002f00: 7020 6661 696c 6564 3a20 2564 0a00 756e  p failed: %d..un
+00002f10: 686f 6f6b 2065 7272 6f72 3a20 2564 0a00  hook error: %d..
+00002f20: 5b2b 5d20 496e 6a65 6374 696e 6720 7072  [+] Injecting pr
+00002f30: 6f63 6573 733a 2025 640a 005f 5f64 6c5f  ocess: %d..__dl_
+00002f40: 5f5f 6c6f 6164 6572 5f64 6c6f 7065 6e00  __loader_dlopen.
+00002f50: 5f5f 646c 5f5f 5a38 5f5f 646c 6f70 656e  __dl__Z8__dlopen
+00002f60: 504b 6369 504b 7600 5f5f 6c6f 6164 6572  PKciPKv.__loader
+00002f70: 5f64 6c6f 7065 6e00 4765 7420 646c 6f70  _dlopen.Get dlop
+00002f80: 656e 2061 6464 7265 7373 2066 6169 6c65  en address faile
+00002f90: 640a 0064 6c6f 7065 6e20 2573 2065 7272  d..dlopen %s err
+00002fa0: 6f72 3a20 2564 0a00 4765 7420 6675 6e63  or: %d..Get func
+00002fb0: 7469 6f6e 2025 7320 696e 2025 7320 6661  tion %s in %s fa
+00002fc0: 696c 6564 0a00 4c6f 6164 206d 6f64 756c  iled..Load modul
+00002fd0: 6520 2573 2066 6169 6c65 640a 0064 6c63  e %s failed..dlc
+00002fe0: 6c6f 7365 0072 6561 646c 696e 6b20 005b  lose.readlink .[
+00002ff0: 2b5d 6c69 6263 5f70 6174 683a 2025 730a  +]libc_path: %s.
+00003000: 005b 2b5d 6c69 6e6b 6572 5f70 6174 683a  .[+]linker_path:
+00003010: 2025 730a 005b 2b5d 6c69 6264 6c5f 7061   %s..[+]libdl_pa
+00003020: 7468 3a20 2573 0a00 5072 6f63 6573 7320  th: %s..Process 
+00003030: 2573 206e 6f74 2066 6f75 6e64 0a00 4d61  %s not found..Ma
+00003040: 7820 7375 7070 6f72 7420 3130 2070 6172  x support 10 par
+00003050: 616d 7300 703a 6d3a 653a 503a 6800 5461  ams.p:m:e:P:h.Ta
+00003060: 7267 6574 2070 726f 6365 7373 206e 6f74  rget process not
+00003070: 2073 7065 6369 6669 6564 0a00 5072 6f63   specified..Proc
+00003080: 6573 7320 2573 2070 6964 3a20 2564 0a00  ess %s pid: %d..
+00003090: 5b2b 5d20 4265 666f 7265 2074 6f20 696e  [+] Before to in
+000030a0: 6a65 6374 2e00 5b2b 5d20 4265 666f 7265  ject..[+] Before
+000030b0: 2074 6f20 696e 6a65 6374 2e0a 005b 2b5d   to inject...[+]
+000030c0: 2049 6e6a 6563 7420 5375 6363 6573 732e   Inject Success.
+000030d0: 005b 2b5d 2049 6e6a 6563 7420 5375 6363  .[+] Inject Succ
+000030e0: 6573 732e 0a00 5b2b 5d20 496e 6a65 6374  ess...[+] Inject
+000030f0: 2046 6169 6c65 642e 005b 2b5d 2049 6e6a   Failed..[+] Inj
+00003100: 6563 7420 4661 696c 6564 2e0a 0070 726f  ect Failed...pro
+00003110: 6365 7373 006d 6f64 756c 6500 656e 7472  cess.module.entr
+00003120: 7900 7061 7261 6d73 0068 656c 7000 0000  y.params.help...
+00003130: 7074 7261 6365 5f67 6574 7265 6773 3a20  ptrace_getregs: 
+00003140: 4361 6e20 6e6f 7420 6765 7420 7265 6769  Can not get regi
+00003150: 7374 6572 2076 616c 7565 7300 7074 7261  ster values.ptra
+00003160: 6365 5f73 6574 7265 6773 3a20 4361 6e20  ce_setregs: Can 
+00003170: 6e6f 7420 7365 7420 7265 6769 7374 6572  not set register
+00003180: 2076 616c 7565 7300 7379 6d74 6162 5f6f   values.symtab_o
+00003190: 6666 7365 743d 3078 2578 2073 796d 7461  ffset=0x%x symta
+000031a0: 625f 656e 7472 6965 733d 3078 2578 2073  b_entries=0x%x s
+000031b0: 7472 7461 625f 6f66 6673 6574 3d30 7825  trtab_offset=0x%
+000031c0: 7800 0000 5b2b 5d20 4361 6c6c 696e 6720  x...[+] Calling 
+000031d0: 6d6d 6170 2069 6e20 7461 7267 6574 2070  mmap in target p
+000031e0: 726f 6365 7373 2025 642e 0a00 5b2b 5d20  rocess %d...[+] 
+000031f0: 496e 6c69 6e65 2068 6f6f 6b20 6973 2064  Inline hook is d
+00003200: 6574 6563 7465 643a 2025 705b 2564 5d20  etected: %p[%d] 
+00003210: 0a00 0000 416c 6c6f 6320 6d65 6d6f 7279  ....Alloc memory
+00003220: 2069 6e20 7461 7267 6574 2070 726f 6365   in target proce
+00003230: 7373 2066 6169 6c65 640a 0000 5b2b 5d20  ss failed...[+] 
+00003240: 4361 6c6c 696e 6720 646c 6f70 656e 2025  Calling dlopen %
+00003250: 7320 696e 2074 6172 6765 7420 7072 6f63  s in target proc
+00003260: 6573 732e 0a00 0000 5b2b 5d20 4361 6c6c  ess.....[+] Call
+00003270: 696e 6720 646c 6f70 656e 2072 6574 7572  ing dlopen retur
+00003280: 6e3a 2025 700a 0000 5b2b 5d20 5265 6d6f  n: %p...[+] Remo
+00003290: 7465 206d 6f64 756c 6520 2573 2061 6464  te module %s add
+000032a0: 723a 2025 700a 0000 5b2b 5d20 5265 6d6f  r: %p...[+] Remo
+000032b0: 7465 2066 756e 6374 696f 6e20 2573 2061  te function %s a
+000032c0: 6464 723a 2025 700a 0000 0000 5b2b 5d20  ddr: %p.....[+] 
+000032d0: 4361 6c6c 696e 6720 6675 6e63 7469 6f6e  Calling function
+000032e0: 2025 7320 696e 2074 6172 6765 7420 7072   %s in target pr
+000032f0: 6f63 6573 732e 0a00 5b2b 5d20 4361 6c6c  ocess...[+] Call
+00003300: 696e 6720 7461 7267 6574 2066 756e 6374  ing target funct
+00003310: 696f 6e20 7265 7475 726e 3a20 3078 256c  ion return: 0x%l
+00003320: 780a 0000 5b2b 5d20 4765 7420 696d 706f  x...[+] Get impo
+00003330: 7274 733a 2064 6c6f 7065 6e3a 2025 702c  rts: dlopen: %p,
+00003340: 2064 6c63 6c6f 7365 3a20 2570 0a00 0000   dlclose: %p....
+00003350: 5573 6167 653a 200a 2020 2020 2e2f 6472  Usage: .    ./dr
+00003360: 6f69 645f 696e 6a65 6374 202d 7020 3c74  oid_inject -p <t
+00003370: 6172 6765 7420 7072 6f63 6573 7320 6e61  arget process na
+00003380: 6d65 206f 7220 6964 3e20 2d6d 203c 7461  me or id> -m <ta
+00003390: 7267 6574 2069 6e6a 6563 7420 6d6f 6475  rget inject modu
+000033a0: 6c65 2070 6174 683e 202d 6520 3c6d 6f64  le path> -e <mod
+000033b0: 756c 6520 656e 7472 7920 6675 6e63 6974  ule entry funcit
+000033c0: 6f6e 3e20 5b2d 5020 7061 7261 6d20 6f66  on> [-P param of
+000033d0: 206d 6f64 756c 6520 656e 7472 7920 6675   module entry fu
+000033e0: 6e63 6974 6f6e 5d0a 0000 0000 5461 7267  nciton].....Targ
+000033f0: 6574 2069 6e6a 6563 7420 6d6f 6475 6c65  et inject module
+00003400: 206e 6f74 2073 7065 6369 6669 6564 0a00   not specified..
+00003410: 456e 7472 7920 6675 6e63 7469 6f6e 206f  Entry function o
+00003420: 6620 6d6f 6475 6c65 2025 7320 6e6f 7420  f module %s not 
+00003430: 7370 6563 6966 6965 640a 0000 5bbe ffff  specified...[...
+00003440: 82be ffff 82be ffff 82be ffff 82be ffff  ................
+00003450: 82be ffff 82be ffff 82be ffff 82be ffff  ................
+00003460: 82be ffff 82be ffff 82be ffff 82be ffff  ................
+00003470: 82be ffff 82be ffff 82be ffff 82be ffff  ................
+00003480: 82be ffff 82be ffff 82be ffff 82be ffff  ................
+00003490: 4abe ffff 82be ffff 82be ffff 13be ffff  J...............
+000034a0: 82be ffff 82be ffff 82be ffff 82be ffff  ................
+000034b0: 02be ffff 82be ffff 82be ffff bebd ffff  ................
+000034c0: 1400 0000 0000 0000 017a 5200 017c 0801  .........zR..|..
+000034d0: 1b0c 0404 8801 0000 1400 0000 1c00 0000  ................
+000034e0: 90db ffff 1300 0000 0044 0e10 4e0e 0400  .........D..N...
+000034f0: 1800 0000 3400 0000 98db ffff 5900 0000  ....4.......Y...
+00003500: 0041 0e08 8502 420d 0541 8303 1c00 0000  .A....B..A......
+00003510: 5000 0000 dcdb ffff 3600 0000 0041 0e08  P.......6....A..
+00003520: 8302 4f0e 2064 0e08 41c3 0e04 1c00 0000  ..O. d..A.......
+00003530: 7000 0000 fcdb ffff 1b00 0000 0041 0e08  p............A..
+00003540: 8302 4f0e 1049 0e08 41c3 0e04 1000 0000  ..O..I..A.......
+00003550: 9000 0000 f7db ffff 0400 0000 0000 0000  ................
+00003560: 3400 0000 a400 0000 e8db ffff b600 0000  4...............
+00003570: 0041 0e08 8702 410e 0c86 0341 0e10 8304  .A....A....A....
+00003580: 4f0e 3002 9b0a 0e10 41c3 0e0c 41c6 0e08  O.0.....A...A...
+00003590: 41c7 0e04 410b 0000 3800 0000 dc00 0000  A...A...8.......
+000035a0: 70dc ffff d800 0000 0041 0e08 8502 410e  p........A....A.
+000035b0: 0c87 0341 0e10 8604 410e 1483 054f 0e50  ...A....A....O.P
+000035c0: 02be 0e14 43c3 0e10 41c6 0e0c 41c7 0e08  ....C...A...A...
+000035d0: 41c5 0e04 5000 0000 1801 0000 14dd ffff  A...P...........
+000035e0: 1d01 0000 0041 0e08 8502 410e 0c87 0341  .....A....A....A
+000035f0: 0e10 8604 410e 1483 054f 0e50 028c 0a0e  ....A....O.P....
+00003600: 1443 c30e 1041 c60e 0c41 c70e 0841 c50e  .C...A...A...A..
+00003610: 0443 0b02 6e0e 1443 c30e 1041 c60e 0c41  .C..n..C...A...A
+00003620: c70e 0841 c50e 0400 3800 0000 6c01 0000  ...A....8...l...
+00003630: e0dd ffff 9700 0000 0041 0e08 8502 410e  .........A....A.
+00003640: 0c87 0341 0e10 8604 410e 1483 054f 0e40  ...A....A....O.@
+00003650: 027f 0e14 41c3 0e10 41c6 0e0c 41c7 0e08  ....A...A...A...
+00003660: 41c5 0e04 2000 0000 a801 0000 44de ffff  A... .......D...
+00003670: 5500 0000 0041 0e08 8302 4f0e 206e 0a0e  U....A....O. n..
+00003680: 0841 c30e 0441 0b00 2000 0000 cc01 0000  .A...A.. .......
+00003690: 80de ffff 5500 0000 0041 0e08 8302 4f0e  ....U....A....O.
+000036a0: 206e 0a0e 0841 c30e 0441 0b00 3000 0000   n...A...A..0...
+000036b0: f001 0000 bcde ffff 5c00 0000 0041 0e08  ........\....A..
+000036c0: 8502 410e 0c87 0341 0e10 8604 440e 7002  ..A....A....D.p.
+000036d0: 4f0e 1043 c60e 0c41 c70e 0841 c50e 0400  O..C...A...A....
+000036e0: 2000 0000 2402 0000 e8de ffff 5500 0000   ...$.......U...
+000036f0: 0041 0e08 8302 4f0e 206e 0a0e 0841 c30e  .A....O. n...A..
+00003700: 0441 0b00 5000 0000 4802 0000 24df ffff  .A..P...H...$...
+00003710: 4601 0000 0041 0e08 8502 430e 0c87 0341  F....A....C....A
+00003720: 0e10 8604 410e 1483 054f 0e50 0317 010a  ....A....O.P....
+00003730: 0e14 41c3 0e10 41c6 0e0c 41c7 0e08 41c5  ..A...A...A...A.
+00003740: 0e04 480b 440e 1446 c30e 1041 c60e 0c41  ..H.D..F...A...A
+00003750: c70e 0841 c50e 0400 2000 0000 9c02 0000  ...A.... .......
+00003760: 20e0 ffff 5500 0000 0041 0e08 8302 4f0e   ...U....A....O.
+00003770: 206e 0a0e 0841 c30e 0441 0b00 3c00 0000   n...A...A..<...
+00003780: c002 0000 5ce0 ffff 0d02 0000 0041 0e08  ....\........A..
+00003790: 8502 410e 0c87 0341 0e10 8604 410e 1483  ..A....A....A...
+000037a0: 054f 0e40 03b9 010a 0e14 41c3 0e10 41c6  .O.@......A...A.
+000037b0: 0e0c 41c7 0e08 41c5 0e04 480b 3c00 0000  ..A...A...H.<...
+000037c0: 0003 0000 2ce2 ffff 4501 0000 0041 0e08  ....,...E....A..
+000037d0: 8502 410e 0c87 0341 0e10 8604 410e 1483  ..A....A....A...
+000037e0: 0552 0ee0 0802 b80a 0e14 41c3 0e10 41c6  .R........A...A.
+000037f0: 0e0c 41c7 0e08 41c5 0e04 460b 2800 0000  ..A...A...F.(...
+00003800: 4003 0000 3ce3 ffff 3900 0000 0041 0e08  @...<...9....A..
+00003810: 8702 410e 0c86 0344 0e20 6e0e 0c41 c60e  ..A....D. n..A..
+00003820: 0843 c70e 0400 0000 8000 0000 6c03 0000  .C..........l...
+00003830: 50e3 ffff cf02 0000 0041 0e08 8502 410e  P........A....A.
+00003840: 0c87 0341 0e10 8604 410e 1483 0552 0eb0  ...A....A....R..
+00003850: 0103 ba01 0a0e 1441 c30e 1041 c60e 0c41  .......A...A...A
+00003860: c70e 0841 c50e 0444 0b02 900a 0e14 43c3  ...A...D......C.
+00003870: 0e10 41c6 0e0c 41c7 0e08 41c5 0e04 410b  ..A...A...A...A.
+00003880: 680a 0e14 43c3 0e10 41c6 0e0c 41c7 0e08  h...C...A...A...
+00003890: 41c5 0e04 410b 530a 0e14 43c3 0e10 41c6  A...A.S...C...A.
+000038a0: 0e0c 41c7 0e08 41c5 0e04 410b 5000 0000  ..A...A...A.P...
+000038b0: f003 0000 9ce5 ffff fd00 0000 0041 0e08  .............A..
+000038c0: 8502 410e 0c87 0341 0e10 8604 410e 1483  ..A....A....A...
+000038d0: 054f 0e40 027e 0a0e 1441 c30e 1041 c60e  .O.@.~...A...A..
+000038e0: 0c41 c70e 0841 c50e 0443 0b02 5e0e 1443  .A...A...C..^..C
+000038f0: c30e 1041 c60e 0c41 c70e 0841 c50e 0400  ...A...A...A....
+00003900: 3c00 0000 4404 0000 48e6 ffff 3a01 0000  <...D...H...:...
+00003910: 0041 0e08 8502 410e 0c87 0341 0e10 8604  .A....A....A....
+00003920: 410e 1483 0552 0ef0 0202 8c0a 0e14 41c3  A....R........A.
+00003930: 0e10 41c6 0e0c 41c7 0e08 41c5 0e04 420b  ..A...A...A...B.
+00003940: 3c00 0000 8404 0000 48e7 ffff d001 0000  <.......H.......
+00003950: 0041 0e08 8502 410e 0c87 0341 0e10 8604  .A....A....A....
+00003960: 410e 1483 054f 0e70 03b6 010e 1443 c30e  A....O.p.....C..
+00003970: 1041 c60e 0c41 c70e 0841 c50e 0400 0000  .A...A...A......
+00003980: 3c00 0000 c404 0000 d8e8 ffff ec00 0000  <...............
+00003990: 0041 0e08 8502 410e 0c87 0341 0e10 8604  .A....A....A....
+000039a0: 410e 1483 054f 0e90 0102 d40e 1441 c30e  A....O.......A..
+000039b0: 1041 c60e 0c41 c70e 0841 c50e 0400 0000  .A...A...A......
+000039c0: 3c00 0000 0405 0000 88e9 ffff f700 0000  <...............
+000039d0: 0041 0e08 8502 410e 0c87 0341 0e10 8604  .A....A....A....
+000039e0: 410e 1483 054f 0e40 02a9 0a0e 1443 c30e  A....O.@.....C..
+000039f0: 1041 c60e 0c41 c70e 0841 c50e 0446 0b00  .A...A...A...F..
+00003a00: 3c00 0000 4405 0000 48ea ffff 2d01 0000  <...D...H...-...
+00003a10: 0041 0e08 8502 460e 0c87 0341 0e10 8604  .A....F....A....
+00003a20: 410e 1483 0552 0ed0 0202 df0a 0e14 41c3  A....R........A.
+00003a30: 0e10 41c6 0e0c 41c7 0e08 41c5 0e04 420b  ..A...A...A...B.
+00003a40: 4000 0000 8405 0000 38eb ffff e106 0000  @.......8.......
+00003a50: 0041 0e08 8502 410e 0c87 0341 0e10 8604  .A....A....A....
+00003a60: 410e 1483 0552 0e80 0203 8702 0a0e 1443  A....R.........C
+00003a70: c30e 1041 c60e 0c41 c70e 0841 c50e 0445  ...A...A...A...E
+00003a80: 0b00 0000 4000 0000 c805 0000 e4f1 ffff  ....@...........
+00003a90: 5e00 0000 0041 0e08 8702 410e 0c86 0341  ^....A....A....A
+00003aa0: 0e10 8304 4f0e 206f 0a0e 1041 c30e 0c41  ....O. o...A...A
+00003ab0: c60e 0841 c70e 0444 0b52 0e10 41c3 0e0c  ...A...D.R..A...
+00003ac0: 41c6 0e08 41c7 0e04 3400 0000 0c06 0000  A...A...4.......
+00003ad0: 00f2 ffff 5b00 0000 0041 0e08 8602 410e  ....[....A....A.
+00003ae0: 0c83 034f 0e80 016b 0a0e 0c41 c30e 0841  ...O...k...A...A
+00003af0: c60e 0442 0b58 0e0c 41c3 0e08 41c6 0e04  ...B.X..A...A...
+00003b00: 2c00 0000 4406 0000 78d0 ffff e404 0000  ,...D...x.......
+00003b10: 0041 0e08 8502 470d 0543 8703 8604 8305  .A....G..C......
+00003b20: 030f 020a c341 c641 c741 c50c 0404 410b  .....A.A.A....A.
+00003b30: 2400 0000 7406 0000 b8cd ffff 9002 0000  $...t...........
+00003b40: 000e 0846 0e0c 4a0f 0b74 0478 003f 1a3b  ...F..J..t.x.?.;
+00003b50: 2a32 2422 0000 0000 0000 0000 011b 033b  *2$"...........;
+00003b60: 60f9 ffff 1e00 0000 94cd ffff d4ff ffff  `...............
+00003b70: 24d0 ffff a4ff ffff 14d5 ffff 7cf9 ffff  $...........|...
+00003b80: 34d5 ffff 94f9 ffff 94d5 ffff b0f9 ffff  4...............
+00003b90: d4d5 ffff d0f9 ffff efd5 ffff f0f9 ffff  ................
+00003ba0: f4d5 ffff 04fa ffff b4d6 ffff 3cfa ffff  ............<...
+00003bb0: 94d7 ffff 78fa ffff b4d8 ffff ccfa ffff  ....x...........
+00003bc0: 54d9 ffff 08fb ffff b4d9 ffff 2cfb ffff  T...........,...
+00003bd0: 14da ffff 50fb ffff 74da ffff 84fb ffff  ....P...t.......
+00003be0: d4da ffff a8fb ffff 24dc ffff fcfb ffff  ........$.......
+00003bf0: 84dc ffff 20fc ffff 94de ffff 60fc ffff  .... .......`...
+00003c00: e4df ffff a0fc ffff 24e0 ffff ccfc ffff  ........$.......
+00003c10: f4e2 ffff 50fd ffff f4e3 ffff a4fd ffff  ....P...........
+00003c20: 34e5 ffff e4fd ffff 04e7 ffff 24fe ffff  4...........$...
+00003c30: f4e7 ffff 64fe ffff f4e8 ffff a4fe ffff  ....d...........
+00003c40: 24ea ffff e4fe ffff 14f1 ffff 28ff ffff  $...........(...
+00003c50: 74f1 ffff 6cff ffff 0000 0000 0000 0000  t...l...........
+00003c60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003c70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003c80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003c90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003ca0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003cb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003cc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003cd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003ce0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003cf0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003d00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003d10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003d20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003d30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003d40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003d50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003d60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003d70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003d80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003d90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003da0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003db0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003dc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003dd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003de0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003df0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003e00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003e10: 0000 0000 ffff ffff 0000 0000 ffff ffff  ................
+00003e20: 0000 0000 ffff ffff 0000 0000 0300 0000  ................
+00003e30: 544f 0000 0200 0000 4001 0000 1700 0000  TO......@.......
+00003e40: a807 0000 1400 0000 1100 0000 1100 0000  ................
+00003e50: 4007 0000 1200 0000 6800 0000 1300 0000  @.......h.......
+00003e60: 0800 0000 faff ff6f 0900 0000 1500 0000  .......o........
+00003e70: 0000 0000 0600 0000 4801 0000 0b00 0000  ........H.......
+00003e80: 1000 0000 0500 0000 3804 0000 0a00 0000  ........8.......
+00003e90: b001 0000 0400 0000 e805 0000 0100 0000  ................
+00003ea0: 8001 0000 0100 0000 8a01 0000 0100 0000  ................
+00003eb0: 9701 0000 0100 0000 9f01 0000 0100 0000  ................
+00003ec0: a701 0000 1a00 0000 144e 0000 1c00 0000  .........N......
+00003ed0: 0800 0000 1900 0000 1c4e 0000 1b00 0000  .........N......
+00003ee0: 0800 0000 2000 0000 244e 0000 2100 0000  .... ...$N..!...
+00003ef0: 0800 0000 1e00 0000 0800 0000 fbff ff6f  ...............o
+00003f00: 0100 0000 0000 0000 0000 0000 0000 0000  ................
+00003f10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003f20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003f30: 0000 0000 244e 0000 1c4e 0000 144e 0000  ....$N...N...N..
+00003f40: 800b 0000 0000 0000 0000 0000 0000 0000  ................
+00003f50: 0000 0000 2c4e 0000 0000 0000 0000 0000  ....,N..........
+00003f60: 0609 0000 1609 0000 2609 0000 3609 0000  ........&...6...
+00003f70: 4609 0000 5609 0000 6609 0000 7609 0000  F...V...f...v...
+00003f80: 8609 0000 9609 0000 a609 0000 b609 0000  ................
+00003f90: c609 0000 d609 0000 e609 0000 f609 0000  ................
+00003fa0: 060a 0000 160a 0000 260a 0000 360a 0000  ........&...6...
+00003fb0: 460a 0000 560a 0000 660a 0000 760a 0000  F...V...f...v...
+00003fc0: 860a 0000 960a 0000 a60a 0000 b60a 0000  ................
+00003fd0: c60a 0000 d60a 0000 e60a 0000 f60a 0000  ................
+00003fe0: 060b 0000 160b 0000 260b 0000 360b 0000  ........&...6...
+00003ff0: 460b 0000 560b 0000 660b 0000 760b 0000  F...V...f...v...
+00004000: 0d31 0000 0100 0000 0000 0000 7000 0000  .1..........p...
+00004010: 1531 0000 0100 0000 0000 0000 6d00 0000  .1..........m...
+00004020: 1c31 0000 0100 0000 0000 0000 6500 0000  .1..........e...
+00004030: 2231 0000 0100 0000 0000 0000 5000 0000  "1..........P...
+00004040: 2931 0000 0000 0000 0000 0000 6800 0000  )1..........h...
+00004050: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004060: 0901 0000 0000 0000 0000 0000 0000 0000  ................
+00004070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004080: 2f73 7973 7465 6d2f 6c69 622f 6c69 6264  /system/lib/libd
+00004090: 6c2e 736f 0000 0000 0000 0000 0000 0000  l.so............
+000040a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000040b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000040c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000040d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000040e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000040f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004100: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004110: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004120: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004130: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004140: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004150: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004160: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004170: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004180: 2f73 7973 7465 6d2f 6269 6e2f 6c69 6e6b  /system/bin/link
+00004190: 6572 0000 0000 0000 0000 0000 0000 0000  er..............
+000041a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000041b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000041c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000041d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000041e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000041f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004230: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004240: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004250: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004260: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004270: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004280: 2f73 7973 7465 6d2f 6c69 622f 6c69 6263  /system/lib/libc
+00004290: 2e73 6f00 0000 0000 0000 0000 0000 0000  .so.............
+000042a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000042b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000042c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000042d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000042e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000042f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004300: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004310: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004320: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004330: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004340: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004350: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004370: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004380: 0047 4343 3a20 2847 4e55 2920 342e 3800  .GCC: (GNU) 4.8.
+00004390: 0400 0000 0900 0000 0400 0000 474e 5500  ............GNU.
+000043a0: 676f 6c64 2031 2e31 3100 0000 002e 7368  gold 1.11.....sh
+000043b0: 7374 7274 6162 002e 696e 7465 7270 002e  strtab..interp..
+000043c0: 6479 6e73 796d 002e 6479 6e73 7472 002e  dynsym..dynstr..
+000043d0: 6861 7368 002e 7265 6c2e 6479 6e00 2e72  hash..rel.dyn..r
+000043e0: 656c 2e70 6c74 002e 7465 7874 002e 6e6f  el.plt..text..no
+000043f0: 7465 2e61 6e64 726f 6964 2e69 6465 6e74  te.android.ident
+00004400: 002e 726f 6461 7461 002e 6568 5f66 7261  ..rodata..eh_fra
+00004410: 6d65 002e 6568 5f66 7261 6d65 5f68 6472  me..eh_frame_hdr
+00004420: 002e 6669 6e69 5f61 7272 6179 002e 696e  ..fini_array..in
+00004430: 6974 5f61 7272 6179 002e 7072 6569 6e69  it_array..preini
+00004440: 745f 6172 7261 7900 2e64 796e 616d 6963  t_array..dynamic
+00004450: 002e 676f 7400 2e67 6f74 2e70 6c74 002e  ..got..got.plt..
+00004460: 6461 7461 002e 6273 7300 2e63 6f6d 6d65  data..bss..comme
+00004470: 6e74 002e 6e6f 7465 2e67 6e75 2e67 6f6c  nt..note.gnu.gol
+00004480: 642d 7665 7273 696f 6e00 0000 0000 0000  d-version.......
+00004490: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000044a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000044b0: 0000 0000 0b00 0000 0100 0000 0200 0000  ................
+000044c0: 3401 0000 3401 0000 1300 0000 0000 0000  4...4...........
+000044d0: 0000 0000 0100 0000 0000 0000 1300 0000  ................
+000044e0: 0b00 0000 0200 0000 4801 0000 4801 0000  ........H...H...
+000044f0: f002 0000 0300 0000 0100 0000 0400 0000  ................
+00004500: 1000 0000 1b00 0000 0300 0000 0200 0000  ................
+00004510: 3804 0000 3804 0000 b001 0000 0000 0000  8...8...........
+00004520: 0000 0000 0100 0000 0000 0000 2300 0000  ............#...
+00004530: 0500 0000 0200 0000 e805 0000 e805 0000  ................
+00004540: 5801 0000 0200 0000 0000 0000 0400 0000  X...............
+00004550: 0400 0000 2900 0000 0900 0000 0200 0000  ....)...........
+00004560: 4007 0000 4007 0000 6800 0000 0200 0000  @...@...h.......
+00004570: 0000 0000 0400 0000 0800 0000 3200 0000  ............2...
+00004580: 0900 0000 4200 0000 a807 0000 a807 0000  ....B...........
+00004590: 4001 0000 0200 0000 0700 0000 0400 0000  @...............
+000045a0: 0800 0000 3600 0000 0100 0000 0600 0000  ....6...........
+000045b0: f008 0000 f008 0000 9002 0000 0000 0000  ................
+000045c0: 0000 0000 1000 0000 0400 0000 3b00 0000  ............;...
+000045d0: 0100 0000 0600 0000 800b 0000 800b 0000  ................
+000045e0: b021 0000 0000 0000 0000 0000 1000 0000  .!..............
+000045f0: 0000 0000 4100 0000 0100 0000 0200 0000  ....A...........
+00004600: 302d 0000 302d 0000 1800 0000 0000 0000  0-..0-..........
+00004610: 0000 0000 0400 0000 0000 0000 5500 0000  ............U...
+00004620: 0100 0000 0200 0000 482d 0000 482d 0000  ........H-..H-..
+00004630: 7807 0000 0000 0000 0000 0000 0400 0000  x...............
+00004640: 0000 0000 5d00 0000 0100 0000 0200 0000  ....]...........
+00004650: c034 0000 c034 0000 9c06 0000 0000 0000  .4...4..........
+00004660: 0000 0000 0400 0000 0000 0000 6700 0000  ............g...
+00004670: 0100 0000 0200 0000 5c3b 0000 5c3b 0000  ........\;..\;..
+00004680: fc00 0000 0000 0000 0000 0000 0400 0000  ................
+00004690: 0000 0000 7500 0000 0f00 0000 0300 0000  ....u...........
+000046a0: 144e 0000 143e 0000 0800 0000 0000 0000  .N...>..........
+000046b0: 0000 0000 0400 0000 0000 0000 8100 0000  ................
+000046c0: 0e00 0000 0300 0000 1c4e 0000 1c3e 0000  .........N...>..
+000046d0: 0800 0000 0000 0000 0000 0000 0400 0000  ................
+000046e0: 0000 0000 8d00 0000 1000 0000 0300 0000  ................
+000046f0: 244e 0000 243e 0000 0800 0000 0000 0000  $N..$>..........
+00004700: 0000 0000 0400 0000 0000 0000 9c00 0000  ................
+00004710: 0600 0000 0300 0000 2c4e 0000 2c3e 0000  ........,N..,>..
+00004720: 0801 0000 0300 0000 0000 0000 0400 0000  ................
+00004730: 0800 0000 a500 0000 0100 0000 0300 0000  ................
+00004740: 344f 0000 343f 0000 2000 0000 0000 0000  4O..4?.. .......
+00004750: 0000 0000 0400 0000 0000 0000 aa00 0000  ................
+00004760: 0100 0000 0300 0000 544f 0000 543f 0000  ........TO..T?..
+00004770: ac00 0000 0000 0000 0000 0000 0400 0000  ................
+00004780: 0000 0000 b300 0000 0100 0000 0300 0000  ................
+00004790: 0050 0000 0040 0000 8003 0000 0000 0000  .P...@..........
+000047a0: 0000 0000 2000 0000 0000 0000 b900 0000  .... ...........
+000047b0: 0800 0000 0300 0000 8053 0000 8043 0000  .........S...C..
+000047c0: 0800 0000 0000 0000 0000 0000 0400 0000  ................
+000047d0: 0000 0000 be00 0000 0100 0000 3000 0000  ............0...
+000047e0: 0000 0000 8043 0000 1000 0000 0000 0000  .....C..........
+000047f0: 0000 0000 0100 0000 0100 0000 c700 0000  ................
+00004800: 0700 0000 0000 0000 0000 0000 9043 0000  .............C..
+00004810: 1c00 0000 0000 0000 0000 0000 0400 0000  ................
+00004820: 0000 0000 0100 0000 0300 0000 0000 0000  ................
+00004830: 0000 0000 ac43 0000 de00 0000 0000 0000  .....C..........
+00004840: 0000 0000 0100 0000 0000 0000            ............
```

#### readelf --wide --decompress --hex-dump=.eh_frame {}

```diff
@@ -1,55 +1,109 @@
 
 Hex dump of section '.eh_frame':
-  0x00001dcc 14000000 00000000 017a5200 017c0801 .........zR..|..
-  0x00001ddc 1b0c0404 88010000 14000000 1c000000 ................
-  0x00001dec 24edffff 13000000 00440e10 4e0e0400 $........D..N...
-  0x00001dfc 1c000000 34000000 dcecffff 24000000 ....4.......$...
-  0x00001e0c 00410e08 83024f0e 20520e08 41c30e04 .A....O. R..A...
-  0x00001e1c 1c000000 54000000 0cedffff 36000000 ....T.......6...
-  0x00001e2c 00410e08 83024f0e 20640e08 41c30e04 .A....O. d..A...
-  0x00001e3c 1c000000 74000000 2cedffff 1b000000 ....t...,.......
-  0x00001e4c 00410e08 83024f0e 10490e08 41c30e04 .A....O..I..A...
-  0x00001e5c 10000000 94000000 2cedffff 04000000 ........,.......
-  0x00001e6c 00000000 68000000 a8000000 28edffff ....h.......(...
-  0x00001e7c 55030000 00410e08 8502410e 0c870341 U....A....A....A
-  0x00001e8c 0e108604 410e1483 054f0e60 0375020a ....A....O.`.u..
-  0x00001e9c 0e1443c3 0e1041c6 0e0c41c7 0e0841c5 ..C...A...A...A.
-  0x00001eac 0e04420b 02950a0e 1443c30e 1041c60e ..B......C...A..
-  0x00001ebc 0c41c70e 0841c50e 04450b5e 0e1443c3 .A...A...E.^..C.
-  0x00001ecc 0e1041c6 0e0c41c7 0e0841c5 0e040000 ..A...A...A.....
-  0x00001edc 40000000 14010000 1cf0ffff de030000 @...............
-  0x00001eec 00410e08 8502410e 0c870341 0e108604 .A....A....A....
-  0x00001efc 410e1483 05520e80 07032c03 0a0e1441 A....R....,....A
-  0x00001f0c c30e1041 c60e0c41 c70e0841 c50e0442 ...A...A...A...B
-  0x00001f1c 0b000000 1c000000 58010000 b8f3ffff ........X.......
-  0x00001f2c 1b000000 00410e08 83024f0e 10490e08 .....A....O..I..
-  0x00001f3c 41c30e04 1c000000 78010000 b8f3ffff A.......x.......
-  0x00001f4c 25000000 00410e08 83024f0e 20510e08 %....A....O. Q..
-  0x00001f5c 43c30e04 20000000 98010000 c8f3ffff C... ...........
-  0x00001f6c 3d000000 00410e08 83024f0e 8001690e =....A....O...i.
-  0x00001f7c 0841c30e 04000000 3c000000 bc010000 .A......<.......
-  0x00001f8c e4f3ffff e3000000 00410e08 8502410e .........A....A.
-  0x00001f9c 0c870341 0e108604 410e1483 054f0e40 ...A....A....O.@
-  0x00001fac 029c0a0e 1441c30e 1041c60e 0c41c70e .....A...A...A..
-  0x00001fbc 0841c50e 04410b00 3c000000 fc010000 .A...A..<.......
-  0x00001fcc 94f4ffff f5000000 00410e08 8502410e .........A....A.
-  0x00001fdc 0c870341 0e108604 410e1483 05520ec0 ...A....A....R..
-  0x00001fec 0802900a 0e1441c3 0e1041c6 0e0c41c7 ......A...A...A.
-  0x00001ffc 0e0841c5 0e04460b 80000000 3c020000 ..A...F.....<...
-  0x0000200c 54f5ffff a6030000 00410e08 8502410e T........A....A.
-  0x0000201c 0c870341 0e108604 410e1483 05520ec0 ...A....A....R..
-  0x0000202c 01034202 0a0e1441 c30e1041 c60e0c41 ..B....A...A...A
-  0x0000203c c70e0841 c50e0444 0b710a0e 1441c30e ...A...D.q...A..
-  0x0000204c 1041c60e 0c41c70e 0841c50e 04430b02 .A...A...A...C..
-  0x0000205c 960a0e14 43c30e10 41c60e0c 41c70e08 ....C...A...A...
-  0x0000206c 41c50e04 440b6b0a 0e1443c3 0e1041c6 A...D.k...C...A.
-  0x0000207c 0e0c41c7 0e0841c5 0e04410b 54000000 ..A...A...A.T...
-  0x0000208c c0020000 80f8ffff 42010000 00410e08 ........B....A..
-  0x0000209c 8502410e 0c870341 0e108604 410e1483 ..A....A....A...
-  0x000020ac 054f0e40 02460a0e 1441c30e 1041c60e .O.@.F...A...A..
-  0x000020bc 0c41c70e 0841c50e 04430b02 860a0e14 .A...A...C......
-  0x000020cc 41c30e10 41c60e0c 41c70e08 41c50e04 A...A...A...A...
-  0x000020dc 460b0000 24000000 18030000 d8e7ffff F...$...........
-  0x000020ec 20020000 000e0846 0e0c4a0f 0b740478  ......F..J..t.x
-  0x000020fc 003f1a3b 2a322422 00000000 00000000 .?.;*2$"........
+  0x000034c0 14000000 00000000 017a5200 017c0801 .........zR..|..
+  0x000034d0 1b0c0404 88010000 14000000 1c000000 ................
+  0x000034e0 90dbffff 13000000 00440e10 4e0e0400 .........D..N...
+  0x000034f0 18000000 34000000 98dbffff 59000000 ....4.......Y...
+  0x00003500 00410e08 8502420d 05418303 1c000000 .A....B..A......
+  0x00003510 50000000 dcdbffff 36000000 00410e08 P.......6....A..
+  0x00003520 83024f0e 20640e08 41c30e04 1c000000 ..O. d..A.......
+  0x00003530 70000000 fcdbffff 1b000000 00410e08 p............A..
+  0x00003540 83024f0e 10490e08 41c30e04 10000000 ..O..I..A.......
+  0x00003550 90000000 f7dbffff 04000000 00000000 ................
+  0x00003560 34000000 a4000000 e8dbffff b6000000 4...............
+  0x00003570 00410e08 8702410e 0c860341 0e108304 .A....A....A....
+  0x00003580 4f0e3002 9b0a0e10 41c30e0c 41c60e08 O.0.....A...A...
+  0x00003590 41c70e04 410b0000 38000000 dc000000 A...A...8.......
+  0x000035a0 70dcffff d8000000 00410e08 8502410e p........A....A.
+  0x000035b0 0c870341 0e108604 410e1483 054f0e50 ...A....A....O.P
+  0x000035c0 02be0e14 43c30e10 41c60e0c 41c70e08 ....C...A...A...
+  0x000035d0 41c50e04 50000000 18010000 14ddffff A...P...........
+  0x000035e0 1d010000 00410e08 8502410e 0c870341 .....A....A....A
+  0x000035f0 0e108604 410e1483 054f0e50 028c0a0e ....A....O.P....
+  0x00003600 1443c30e 1041c60e 0c41c70e 0841c50e .C...A...A...A..
+  0x00003610 04430b02 6e0e1443 c30e1041 c60e0c41 .C..n..C...A...A
+  0x00003620 c70e0841 c50e0400 38000000 6c010000 ...A....8...l...
+  0x00003630 e0ddffff 97000000 00410e08 8502410e .........A....A.
+  0x00003640 0c870341 0e108604 410e1483 054f0e40 ...A....A....O.@
+  0x00003650 027f0e14 41c30e10 41c60e0c 41c70e08 ....A...A...A...
+  0x00003660 41c50e04 20000000 a8010000 44deffff A... .......D...
+  0x00003670 55000000 00410e08 83024f0e 206e0a0e U....A....O. n..
+  0x00003680 0841c30e 04410b00 20000000 cc010000 .A...A.. .......
+  0x00003690 80deffff 55000000 00410e08 83024f0e ....U....A....O.
+  0x000036a0 206e0a0e 0841c30e 04410b00 30000000  n...A...A..0...
+  0x000036b0 f0010000 bcdeffff 5c000000 00410e08 ........\....A..
+  0x000036c0 8502410e 0c870341 0e108604 440e7002 ..A....A....D.p.
+  0x000036d0 4f0e1043 c60e0c41 c70e0841 c50e0400 O..C...A...A....
+  0x000036e0 20000000 24020000 e8deffff 55000000  ...$.......U...
+  0x000036f0 00410e08 83024f0e 206e0a0e 0841c30e .A....O. n...A..
+  0x00003700 04410b00 50000000 48020000 24dfffff .A..P...H...$...
+  0x00003710 46010000 00410e08 8502430e 0c870341 F....A....C....A
+  0x00003720 0e108604 410e1483 054f0e50 0317010a ....A....O.P....
+  0x00003730 0e1441c3 0e1041c6 0e0c41c7 0e0841c5 ..A...A...A...A.
+  0x00003740 0e04480b 440e1446 c30e1041 c60e0c41 ..H.D..F...A...A
+  0x00003750 c70e0841 c50e0400 20000000 9c020000 ...A.... .......
+  0x00003760 20e0ffff 55000000 00410e08 83024f0e  ...U....A....O.
+  0x00003770 206e0a0e 0841c30e 04410b00 3c000000  n...A...A..<...
+  0x00003780 c0020000 5ce0ffff 0d020000 00410e08 ....\........A..
+  0x00003790 8502410e 0c870341 0e108604 410e1483 ..A....A....A...
+  0x000037a0 054f0e40 03b9010a 0e1441c3 0e1041c6 .O.@......A...A.
+  0x000037b0 0e0c41c7 0e0841c5 0e04480b 3c000000 ..A...A...H.<...
+  0x000037c0 00030000 2ce2ffff 45010000 00410e08 ....,...E....A..
+  0x000037d0 8502410e 0c870341 0e108604 410e1483 ..A....A....A...
+  0x000037e0 05520ee0 0802b80a 0e1441c3 0e1041c6 .R........A...A.
+  0x000037f0 0e0c41c7 0e0841c5 0e04460b 28000000 ..A...A...F.(...
+  0x00003800 40030000 3ce3ffff 39000000 00410e08 @...<...9....A..
+  0x00003810 8702410e 0c860344 0e206e0e 0c41c60e ..A....D. n..A..
+  0x00003820 0843c70e 04000000 80000000 6c030000 .C..........l...
+  0x00003830 50e3ffff cf020000 00410e08 8502410e P........A....A.
+  0x00003840 0c870341 0e108604 410e1483 05520eb0 ...A....A....R..
+  0x00003850 0103ba01 0a0e1441 c30e1041 c60e0c41 .......A...A...A
+  0x00003860 c70e0841 c50e0444 0b02900a 0e1443c3 ...A...D......C.
+  0x00003870 0e1041c6 0e0c41c7 0e0841c5 0e04410b ..A...A...A...A.
+  0x00003880 680a0e14 43c30e10 41c60e0c 41c70e08 h...C...A...A...
+  0x00003890 41c50e04 410b530a 0e1443c3 0e1041c6 A...A.S...C...A.
+  0x000038a0 0e0c41c7 0e0841c5 0e04410b 50000000 ..A...A...A.P...
+  0x000038b0 f0030000 9ce5ffff fd000000 00410e08 .............A..
+  0x000038c0 8502410e 0c870341 0e108604 410e1483 ..A....A....A...
+  0x000038d0 054f0e40 027e0a0e 1441c30e 1041c60e .O.@.~...A...A..
+  0x000038e0 0c41c70e 0841c50e 04430b02 5e0e1443 .A...A...C..^..C
+  0x000038f0 c30e1041 c60e0c41 c70e0841 c50e0400 ...A...A...A....
+  0x00003900 3c000000 44040000 48e6ffff 3a010000 <...D...H...:...
+  0x00003910 00410e08 8502410e 0c870341 0e108604 .A....A....A....
+  0x00003920 410e1483 05520ef0 02028c0a 0e1441c3 A....R........A.
+  0x00003930 0e1041c6 0e0c41c7 0e0841c5 0e04420b ..A...A...A...B.
+  0x00003940 3c000000 84040000 48e7ffff d0010000 <.......H.......
+  0x00003950 00410e08 8502410e 0c870341 0e108604 .A....A....A....
+  0x00003960 410e1483 054f0e70 03b6010e 1443c30e A....O.p.....C..
+  0x00003970 1041c60e 0c41c70e 0841c50e 04000000 .A...A...A......
+  0x00003980 3c000000 c4040000 d8e8ffff ec000000 <...............
+  0x00003990 00410e08 8502410e 0c870341 0e108604 .A....A....A....
+  0x000039a0 410e1483 054f0e90 0102d40e 1441c30e A....O.......A..
+  0x000039b0 1041c60e 0c41c70e 0841c50e 04000000 .A...A...A......
+  0x000039c0 3c000000 04050000 88e9ffff f7000000 <...............
+  0x000039d0 00410e08 8502410e 0c870341 0e108604 .A....A....A....
+  0x000039e0 410e1483 054f0e40 02a90a0e 1443c30e A....O.@.....C..
+  0x000039f0 1041c60e 0c41c70e 0841c50e 04460b00 .A...A...A...F..
+  0x00003a00 3c000000 44050000 48eaffff 2d010000 <...D...H...-...
+  0x00003a10 00410e08 8502460e 0c870341 0e108604 .A....F....A....
+  0x00003a20 410e1483 05520ed0 0202df0a 0e1441c3 A....R........A.
+  0x00003a30 0e1041c6 0e0c41c7 0e0841c5 0e04420b ..A...A...A...B.
+  0x00003a40 40000000 84050000 38ebffff e1060000 @.......8.......
+  0x00003a50 00410e08 8502410e 0c870341 0e108604 .A....A....A....
+  0x00003a60 410e1483 05520e80 02038702 0a0e1443 A....R.........C
+  0x00003a70 c30e1041 c60e0c41 c70e0841 c50e0445 ...A...A...A...E
+  0x00003a80 0b000000 40000000 c8050000 e4f1ffff ....@...........
+  0x00003a90 5e000000 00410e08 8702410e 0c860341 ^....A....A....A
+  0x00003aa0 0e108304 4f0e206f 0a0e1041 c30e0c41 ....O. o...A...A
+  0x00003ab0 c60e0841 c70e0444 0b520e10 41c30e0c ...A...D.R..A...
+  0x00003ac0 41c60e08 41c70e04 34000000 0c060000 A...A...4.......
+  0x00003ad0 00f2ffff 5b000000 00410e08 8602410e ....[....A....A.
+  0x00003ae0 0c83034f 0e80016b 0a0e0c41 c30e0841 ...O...k...A...A
+  0x00003af0 c60e0442 0b580e0c 41c30e08 41c60e04 ...B.X..A...A...
+  0x00003b00 2c000000 44060000 78d0ffff e4040000 ,...D...x.......
+  0x00003b10 00410e08 8502470d 05438703 86048305 .A....G..C......
+  0x00003b20 030f020a c341c641 c741c50c 0404410b .....A.A.A....A.
+  0x00003b30 24000000 74060000 b8cdffff 90020000 $...t...........
+  0x00003b40 000e0846 0e0c4a0f 0b740478 003f1a3b ...F..J..t.x.?.;
+  0x00003b50 2a322422 00000000 00000000          *2$"........
```

#### readelf --wide --decompress --hex-dump=.eh_frame_hdr {}

```diff
@@ -1,12 +1,19 @@
 
 Hex dump of section '.eh_frame_hdr':
-  0x0000210c 011b033b bcfcffff 0f000000 b4e7ffff ...;............
-  0x0000211c d4ffffff d4e9ffff f0fcffff 04eaffff ................
-  0x0000212c d8fcffff 24eaffff 10fdffff 64eaffff ....$.......d...
-  0x0000213c 30fdffff 84eaffff 50fdffff 94eaffff 0.......P.......
-  0x0000214c 64fdffff f4edffff d0fdffff d4f1ffff d...............
-  0x0000215c 14feffff f4f1ffff 34feffff 24f2ffff ........4...$...
-  0x0000216c 54feffff 64f2ffff 78feffff 54f3ffff T...d...x...T...
-  0x0000217c b8feffff 54f4ffff f8feffff 04f8ffff ....T...........
-  0x0000218c 7cffffff                            |...
+  0x00003b5c 011b033b 60f9ffff 1e000000 94cdffff ...;`...........
+  0x00003b6c d4ffffff 24d0ffff a4ffffff 14d5ffff ....$...........
+  0x00003b7c 7cf9ffff 34d5ffff 94f9ffff 94d5ffff |...4...........
+  0x00003b8c b0f9ffff d4d5ffff d0f9ffff efd5ffff ................
+  0x00003b9c f0f9ffff f4d5ffff 04faffff b4d6ffff ................
+  0x00003bac 3cfaffff 94d7ffff 78faffff b4d8ffff <.......x.......
+  0x00003bbc ccfaffff 54d9ffff 08fbffff b4d9ffff ....T...........
+  0x00003bcc 2cfbffff 14daffff 50fbffff 74daffff ,.......P...t...
+  0x00003bdc 84fbffff d4daffff a8fbffff 24dcffff ............$...
+  0x00003bec fcfbffff 84dcffff 20fcffff 94deffff ........ .......
+  0x00003bfc 60fcffff e4dfffff a0fcffff 24e0ffff `...........$...
+  0x00003c0c ccfcffff f4e2ffff 50fdffff f4e3ffff ........P.......
+  0x00003c1c a4fdffff 34e5ffff e4fdffff 04e7ffff ....4...........
+  0x00003c2c 24feffff f4e7ffff 64feffff f4e8ffff $.......d.......
+  0x00003c3c a4feffff 24eaffff e4feffff 14f1ffff ....$...........
+  0x00003c4c 28ffffff 74f1ffff 6cffffff          (...t...l...
```

#### readelf --wide --decompress --hex-dump=.fini_array {}

```diff
@@ -1,4 +1,4 @@
 
 Hex dump of section '.fini_array':
-  0x00003e5c e00a0000 00000000                   ........
+  0x00004e14 ffffffff 00000000                   ........
```

#### readelf --wide --decompress --hex-dump=.init_array {}

```diff
@@ -1,4 +1,4 @@
 
 Hex dump of section '.init_array':
-  0x00003e64 00000000                            ....
+  0x00004e1c ffffffff 00000000                   ........
```

#### readelf --wide --decompress --hex-dump=.got {}

```diff
@@ -1,4 +1,5 @@
 
 Hex dump of section '.got':
-  0x00003f68 00000000 a00b0000                   ........
+  0x00004f34 244e0000 1c4e0000 144e0000 800b0000 $N...N...N......
+  0x00004f44 00000000 00000000 00000000 00000000 ................
```

#### readelf --wide --decompress --hex-dump=.got.plt {}

```diff
@@ -1,12 +1,14 @@
 
 Hex dump of section '.got.plt':
-  0x00003f70 683e0000 00000000 00000000 d6080000 h>..............
-  0x00003f80 e6080000 f6080000 06090000 16090000 ................
-  0x00003f90 26090000 36090000 46090000 56090000 &...6...F...V...
-  0x00003fa0 66090000 76090000 86090000 96090000 f...v...........
-  0x00003fb0 a6090000 b6090000 c6090000 d6090000 ................
-  0x00003fc0 e6090000 f6090000 060a0000 160a0000 ................
-  0x00003fd0 260a0000 360a0000 460a0000 560a0000 &...6...F...V...
-  0x00003fe0 660a0000 760a0000 860a0000 960a0000 f...v...........
-  0x00003ff0 a60a0000 b60a0000 c60a0000 d60a0000 ................
+  0x00004f54 2c4e0000 00000000 00000000 06090000 ,N..............
+  0x00004f64 16090000 26090000 36090000 46090000 ....&...6...F...
+  0x00004f74 56090000 66090000 76090000 86090000 V...f...v.......
+  0x00004f84 96090000 a6090000 b6090000 c6090000 ................
+  0x00004f94 d6090000 e6090000 f6090000 060a0000 ................
+  0x00004fa4 160a0000 260a0000 360a0000 460a0000 ....&...6...F...
+  0x00004fb4 560a0000 660a0000 760a0000 860a0000 V...f...v.......
+  0x00004fc4 960a0000 a60a0000 b60a0000 c60a0000 ................
+  0x00004fd4 d60a0000 e60a0000 f60a0000 060b0000 ................
+  0x00004fe4 160b0000 260b0000 360b0000 460b0000 ....&...6...F...
+  0x00004ff4 560b0000 660b0000 760b0000          V...f...v...
```

#### readelf --wide --decompress --hex-dump=.data {}

```diff
@@ -1,4 +1,59 @@
 
 Hex dump of section '.data':
-  0x00004000 00400000                            .@..
+  0x00005000 0d310000 01000000 00000000 70000000 .1..........p...
+  0x00005010 15310000 01000000 00000000 6d000000 .1..........m...
+  0x00005020 1c310000 01000000 00000000 65000000 .1..........e...
+  0x00005030 22310000 01000000 00000000 50000000 "1..........P...
+  0x00005040 29310000 00000000 00000000 68000000 )1..........h...
+  0x00005050 00000000 00000000 00000000 00000000 ................
+  0x00005060 09010000 00000000 00000000 00000000 ................
+  0x00005070 00000000 00000000 00000000 00000000 ................
+  0x00005080 2f737973 74656d2f 6c69622f 6c696264 /system/lib/libd
+  0x00005090 6c2e736f 00000000 00000000 00000000 l.so............
+  0x000050a0 00000000 00000000 00000000 00000000 ................
+  0x000050b0 00000000 00000000 00000000 00000000 ................
+  0x000050c0 00000000 00000000 00000000 00000000 ................
+  0x000050d0 00000000 00000000 00000000 00000000 ................
+  0x000050e0 00000000 00000000 00000000 00000000 ................
+  0x000050f0 00000000 00000000 00000000 00000000 ................
+  0x00005100 00000000 00000000 00000000 00000000 ................
+  0x00005110 00000000 00000000 00000000 00000000 ................
+  0x00005120 00000000 00000000 00000000 00000000 ................
+  0x00005130 00000000 00000000 00000000 00000000 ................
+  0x00005140 00000000 00000000 00000000 00000000 ................
+  0x00005150 00000000 00000000 00000000 00000000 ................
+  0x00005160 00000000 00000000 00000000 00000000 ................
+  0x00005170 00000000 00000000 00000000 00000000 ................
+  0x00005180 2f737973 74656d2f 62696e2f 6c696e6b /system/bin/link
+  0x00005190 65720000 00000000 00000000 00000000 er..............
+  0x000051a0 00000000 00000000 00000000 00000000 ................
+  0x000051b0 00000000 00000000 00000000 00000000 ................
+  0x000051c0 00000000 00000000 00000000 00000000 ................
+  0x000051d0 00000000 00000000 00000000 00000000 ................
+  0x000051e0 00000000 00000000 00000000 00000000 ................
+  0x000051f0 00000000 00000000 00000000 00000000 ................
+  0x00005200 00000000 00000000 00000000 00000000 ................
+  0x00005210 00000000 00000000 00000000 00000000 ................
+  0x00005220 00000000 00000000 00000000 00000000 ................
+  0x00005230 00000000 00000000 00000000 00000000 ................
+  0x00005240 00000000 00000000 00000000 00000000 ................
+  0x00005250 00000000 00000000 00000000 00000000 ................
+  0x00005260 00000000 00000000 00000000 00000000 ................
+  0x00005270 00000000 00000000 00000000 00000000 ................
+  0x00005280 2f737973 74656d2f 6c69622f 6c696263 /system/lib/libc
+  0x00005290 2e736f00 00000000 00000000 00000000 .so.............
+  0x000052a0 00000000 00000000 00000000 00000000 ................
+  0x000052b0 00000000 00000000 00000000 00000000 ................
+  0x000052c0 00000000 00000000 00000000 00000000 ................
+  0x000052d0 00000000 00000000 00000000 00000000 ................
+  0x000052e0 00000000 00000000 00000000 00000000 ................
+  0x000052f0 00000000 00000000 00000000 00000000 ................
+  0x00005300 00000000 00000000 00000000 00000000 ................
+  0x00005310 00000000 00000000 00000000 00000000 ................
+  0x00005320 00000000 00000000 00000000 00000000 ................
+  0x00005330 00000000 00000000 00000000 00000000 ................
+  0x00005340 00000000 00000000 00000000 00000000 ................
+  0x00005350 00000000 00000000 00000000 00000000 ................
+  0x00005360 00000000 00000000 00000000 00000000 ................
+  0x00005370 00000000 00000000 00000000 00000000 ................
```

#### readelf --wide --decompress --hex-dump=.shstrtab {}

```diff
@@ -1,15 +1,17 @@
 
 Hex dump of section '.shstrtab':
-  0x00000000 002e7368 73747274 6162002e 64796e73 ..shstrtab..dyns
-  0x00000010 796d002e 64796e73 7472002e 68617368 ym..dynstr..hash
-  0x00000020 002e7265 6c2e6479 6e002e72 656c2e70 ..rel.dyn..rel.p
-  0x00000030 6c74002e 74657874 002e726f 64617461 lt..text..rodata
-  0x00000040 002e6568 5f667261 6d65002e 65685f66 ..eh_frame..eh_f
-  0x00000050 72616d65 5f686472 002e6669 6e695f61 rame_hdr..fini_a
-  0x00000060 72726179 002e696e 69745f61 72726179 rray..init_array
-  0x00000070 002e6479 6e616d69 63002e67 6f74002e ..dynamic..got..
-  0x00000080 676f742e 706c7400 2e646174 61002e62 got.plt..data..b
-  0x00000090 7373002e 636f6d6d 656e7400 2e6e6f74 ss..comment..not
-  0x000000a0 652e676e 752e676f 6c642d76 65727369 e.gnu.gold-versi
-  0x000000b0 6f6e00                              on.
+  0x00000000 002e7368 73747274 6162002e 696e7465 ..shstrtab..inte
+  0x00000010 7270002e 64796e73 796d002e 64796e73 rp..dynsym..dyns
+  0x00000020 7472002e 68617368 002e7265 6c2e6479 tr..hash..rel.dy
+  0x00000030 6e002e72 656c2e70 6c74002e 74657874 n..rel.plt..text
+  0x00000040 002e6e6f 74652e61 6e64726f 69642e69 ..note.android.i
+  0x00000050 64656e74 002e726f 64617461 002e6568 dent..rodata..eh
+  0x00000060 5f667261 6d65002e 65685f66 72616d65 _frame..eh_frame
+  0x00000070 5f686472 002e6669 6e695f61 72726179 _hdr..fini_array
+  0x00000080 002e696e 69745f61 72726179 002e7072 ..init_array..pr
+  0x00000090 65696e69 745f6172 72617900 2e64796e einit_array..dyn
+  0x000000a0 616d6963 002e676f 74002e67 6f742e70 amic..got..got.p
+  0x000000b0 6c74002e 64617461 002e6273 73002e63 lt..data..bss..c
+  0x000000c0 6f6d6d65 6e74002e 6e6f7465 2e676e75 omment..note.gnu
+  0x000000d0 2e676f6c 642d7665 7273696f 6e00     .gold-version.
```

### Comparing `qt4a-2.3.1/qt4a/androiddriver/tools/x86/screenkit` & `qt4a-3.0.0/qt4a/androiddriver/tools/x86/screenkit`

 * *Files identical despite different names*

### Comparing `qt4a-2.3.1/qt4a/androiddriver/util.py` & `qt4a-3.0.0/qt4a/androiddriver/util.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,312 +8,340 @@
 # https://opensource.org/licenses/BSD-3-Clause
 #
 # Unless required by applicable law or agreed to in writing, software distributed
 # under the License is distributed on an "AS IS" basis, WITHOUT WARRANTIES OR CONDITIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 #
-'''
+"""
 通用功能模块
-'''
+"""
 
 from __future__ import print_function
 import six
 import logging
 import os
 import sys
 import threading
 import time
 
 
 class Deprecated(object):
-    '''废弃函数包装
-    '''
+    """废弃函数包装"""
 
     def __init__(self, new_func):
         self._new_func = new_func
 
     def __call__(self, func):
         def warp_func(*args, **kwargs):
             frame = sys._getframe(1)
             code = frame.f_code
             file_name = os.path.split(code.co_filename)[-1]
-            print('method %s is deprecated, called in [%s:%s], pls use %s instead' % (func.__name__, file_name, code.co_name, self._new_func), file=sys.stderr)
+            print(
+                "method %s is deprecated, called in [%s:%s], pls use %s instead"
+                % (func.__name__, file_name, code.co_name, self._new_func),
+                file=sys.stderr,
+            )
             return func(*args, **kwargs)
 
         return warp_func
 
 
 class TimeoutError(RuntimeError):
-    '''超时错误
-    '''
+    """超时错误"""
+
     pass
 
 
 class SocketError(RuntimeError):
-    '''Socket连接错误
-    '''
+    """Socket连接错误"""
+
     pass
 
 
 class AndroidSpyError(RuntimeError):
-    '''测试桩返回错误
-    '''
+    """测试桩返回错误"""
+
     pass
 
 
 class ProcessExitError(RuntimeError):
-    '''进程退出错误
-    '''
+    """进程退出错误"""
+
     pass
 
 
 class ControlExpiredError(AndroidSpyError):
-    '''控件失效错误
-    '''
+    """控件失效错误"""
+
     pass
 
 
 class ControlAmbiguousError(AndroidSpyError):
-    '''控件重复错误
-    '''
+    """控件重复错误"""
+
     pass
 
 
 class InstallPackageFailedError(RuntimeError):
-    '''应用安装失败错误
-    '''
+    """应用安装失败错误"""
+
     pass
 
 
 class PackageError(RuntimeError):
-    '''安装包错误
-    '''
+    """安装包错误"""
+
     pass
 
 
 class PermissionError(RuntimeError):
-    '''权限错误
-    '''
+    """权限错误"""
+
     pass
 
 
 class QT4ADriverNotInstalled(Exception):
-    '''QT4A驱动错误
-    '''
+    """QT4A驱动错误"""
+
     pass
 
 
 class OutStream(object):
-    '''重载输出流，以便在cmd中显示中文
-    '''
+    """重载输出流，以便在cmd中显示中文"""
 
     def __init__(self, stdout):
         self._stdout = stdout
 
     @property
     def encoding(self):
-        return 'utf8'
+        return "utf8"
 
     def write(self, s):
         if six.PY2 and (not isinstance(s, unicode)):
             try:
-                s = s.decode('utf8')
+                s = s.decode("utf8")
             except UnicodeDecodeError:
                 try:
-                    s = s.decode('gbk')  # sys.getdefaultencoding()
+                    s = s.decode("gbk")  # sys.getdefaultencoding()
                 except UnicodeDecodeError:
-                    s = 'Decode Error: %r' % s
+                    s = "Decode Error: %r" % s
                     # s = s.encode('raw_unicode_escape') #不能使用GBK编码
         try:
             ret = self._stdout.write(s)
             self.flush()
             return ret
         except UnicodeEncodeError:
             pass
 
     def flush(self):
         return self._stdout.flush()
 
 
 def mkdir(dir_path):
-    '''创建目录
-    '''
-    if os.path.exists(dir_path): return
+    """创建目录"""
+    if os.path.exists(dir_path):
+        return
     try:
         os.makedirs(dir_path)
     except OSError as e:
         if e.args[0] == 183 or e.args[0] == 17:
             # 文件已经存在
             return
         raise e
 
 
 def gen_log_path():
-    '''生成log存放路径
-        优先使用环境变量[LOG_PATH_PREFIX], 若不存在则使用[APPDATA] / [HOME]
-    '''
-    dir_root = os.environ.get('LOG_PATH_PREFIX', os.environ['APPDATA' if sys.platform == 'win32' else 'HOME'])
+    """生成log存放路径
+    优先使用环境变量[LOG_PATH_PREFIX], 若不存在则使用[APPDATA] / [HOME]
+    """
+    dir_root = os.environ.get(
+        "LOG_PATH_PREFIX", os.environ["APPDATA" if sys.platform == "win32" else "HOME"]
+    )
 
-    dir_root = os.path.join(dir_root, 'qt4a')
+    dir_root = os.path.join(dir_root, "qt4a")
     mkdir(dir_root)
     from datetime import datetime, date
+
     dir_root = os.path.join(dir_root, str(date.today()))
     mkdir(dir_root)
     dt = datetime.now()
-    log_name = '%s_%d.log' % (dt.strftime('%H-%M-%S'), threading.current_thread().ident)
+    log_name = "%s_%d.log" % (dt.strftime("%H-%M-%S"), threading.current_thread().ident)
     return os.path.join(dir_root, log_name)
 
 
-logger = logging.getLogger('qt4a')
+logger = logging.getLogger("qt4a")
 logger.setLevel(logging.DEBUG)
 logger.addHandler(logging.StreamHandler(OutStream(sys.stdout)))
-fmt = logging.Formatter('%(asctime)s %(thread)d %(message)s')  # %(filename)s %(funcName)s
+fmt = logging.Formatter(
+    "%(asctime)s %(thread)d %(message)s"
+)  # %(filename)s %(funcName)s
 logger.handlers[0].setFormatter(fmt)
 logger.handlers[0].setLevel(logging.WARNING)  # 屏幕日志级别为WARNING
 # logger.addHandler(logging.StreamHandler(sys.stderr))
 
 logger_path = gen_log_path()
 file_handler = logging.FileHandler(logger_path)
-fmt = logging.Formatter('%(asctime)s %(levelname)s %(thread)d %(message)s')  # %(filename)s %(funcName)s
+fmt = logging.Formatter(
+    "%(asctime)s %(levelname)s %(thread)d %(message)s"
+)  # %(filename)s %(funcName)s
 file_handler.setFormatter(fmt)
 logger.addHandler(file_handler)
 
 
 def clear_logger_file():
-    '''清空log文件
-    '''
+    """清空log文件"""
     if logger_path:
         try:
-            f = open(logger_path, 'w')
-            f.write('')
+            f = open(logger_path, "w")
+            f.write("")
             f.close()
         except:
             pass
 
 
 def get_default_encoding():
     import locale
     import codecs
+
     return codecs.lookup(locale.getpreferredencoding()).name
 
 
-def set_default_encoding(code='utf8'):
-    if six.PY2: 
-        if sys.getdefaultencoding() == code: return
+def set_default_encoding(code="utf8"):
+    if six.PY2:
+        if sys.getdefaultencoding() == code:
+            return
         reload(sys)
         sys.setdefaultencoding(code)
 
 
+def get_command_path(command):
+    sep = ":"
+    if sys.platform == "win32":
+        sep = ";"
+        command += ".exe"
+    path = os.environ.get("PATH")
+    if isinstance(path, bytes):
+        try:
+            path = path.decode("utf8")
+        except UnicodeDecodeError:
+            path = path.decode("gbk")
+    for root in path.split(sep):
+        command_path = os.path.join(root, command)
+        if os.path.isfile(command_path):
+            return command_path
+
+    return None
+
+
 def get_file_md5(file_path):
-    '''计算文件md5
-    '''
+    """计算文件md5"""
     import hashlib
+
     if six.PY2 and (not isinstance(file_path, unicode)):
-        file_path = file_path.decode('utf8')
+        file_path = file_path.decode("utf8")
     if not os.path.exists(file_path):
-        raise RuntimeError('文件：%s 不存在' % file_path)
-    with open(file_path, 'rb') as f:
+        raise RuntimeError("文件：%s 不存在" % file_path)
+    with open(file_path, "rb") as f:
         content = f.read()
         md5 = hashlib.md5()
         md5.update(content)
         return md5.hexdigest()
 
 
 class static_property(property):
-    '''静态属性
-    '''
+    """静态属性"""
 
     def __init__(self, *args, **kwargs):
         super(static_property, self).__init__(*args, **kwargs)
         self._value_dict = {}
 
     def __get__(self, obj, cls):
         if not id(obj) in self._value_dict:
             self._value_dict[id(obj)] = super(static_property, self).__get__(obj, cls)
         return self._value_dict[id(obj)]
 
 
 class AndroidPackage(object):
-    '''APK文件处理类
-    '''
+    """APK文件处理类"""
 
     def __init__(self, package_path):
         self._package_path = package_path
         if not os.path.exists(package_path):
-            raise RuntimeError('安装包: %s 不存在' % package_path)
+            raise RuntimeError("安装包: %s 不存在" % package_path)
         self._file = None
 
     def _get_file(self):
         if not self._file:
             import zipfile
             from io import BytesIO
-            with open(self._package_path, 'rb') as f:
+
+            with open(self._package_path, "rb") as f:
                 apk_data = f.read()
-                self._file = zipfile.ZipFile(BytesIO(apk_data), mode='r')
+                self._file = zipfile.ZipFile(BytesIO(apk_data), mode="r")
         return self._file
 
     def _get_manifest_xml(self):
         from qt4a.androiddriver._axmlparser import AXMLPrinter
+
         f = self._get_file()
         for i in f.namelist():
             if i == "AndroidManifest.xml":
                 return AXMLPrinter(f.read(i)).get_xml_obj()
-        raise PackageError('找不到AndroidManifest.xml文件')
+        raise PackageError("找不到AndroidManifest.xml文件")
 
     @property
     def package_name(self):
-        '''包名
-        '''
+        """包名"""
         manifest = self._get_manifest_xml()
-        return manifest.getElementsByTagName('manifest')[0].getAttribute('package')
+        return manifest.getElementsByTagName("manifest")[0].getAttribute("package")
 
     @property
     def application_name(self):
-        '''应用名
-        '''
+        """应用名"""
         manifest = self._get_manifest_xml()
-        return manifest.getElementsByTagName('application')[0].getAttribute('android:label')
+        return manifest.getElementsByTagName("application")[0].getAttribute(
+            "android:label"
+        )
 
     @property
     def version(self):
-        '''应用版本
-        '''
+        """应用版本"""
         manifest = self._get_manifest_xml()
-        return manifest.getElementsByTagName('manifest')[0].getAttribute('android:versionName')
+        return manifest.getElementsByTagName("manifest")[0].getAttribute(
+            "android:versionName"
+        )
 
     @property
     def start_activity(self):
-        '''启动Activity
-        '''
+        """启动Activity"""
         manifest = self._get_manifest_xml()
-        for activity in manifest.getElementsByTagName('activity'):
-            for filter in activity.getElementsByTagName('action'):
-                if filter.getAttribute('android:name') == 'android.intent.action.MAIN':
-                    return activity.getAttribute('android:name')
-        for activity in manifest.getElementsByTagName('activity-alias'):
-            for filter in activity.getElementsByTagName('action'):
-                if filter.getAttribute('android:name') == 'android.intent.action.MAIN':
-                    return activity.getAttribute('android:targetActivity')
-        raise PackageError('未找到启动Activity')
+        for activity in manifest.getElementsByTagName("activity"):
+            for filter in activity.getElementsByTagName("action"):
+                if filter.getAttribute("android:name") == "android.intent.action.MAIN":
+                    return activity.getAttribute("android:name")
+        for activity in manifest.getElementsByTagName("activity-alias"):
+            for filter in activity.getElementsByTagName("action"):
+                if filter.getAttribute("android:name") == "android.intent.action.MAIN":
+                    return activity.getAttribute("android:targetActivity")
+        raise PackageError("未找到启动Activity")
 
     @property
     def permissions(self):
-        '''应用申请的权限
-        '''
+        """应用申请的权限"""
         result = []
         manifest = self._get_manifest_xml()
-        for item in manifest.getElementsByTagName('uses-permission'):
-            result.append(item.getAttribute('android:name'))
+        for item in manifest.getElementsByTagName("uses-permission"):
+            result.append(item.getAttribute("android:name"))
         return result
 
 
 class KeyCode(object):
-    '''按键对应关系
-    '''
+    """按键对应关系"""
+
     KEYCODE_SOFT_LEFT = 1
     KEYCODE_SOFT_RIGHT = 2
     KEYCODE_HOME = 3
     KEYCODE_BACK = 4
     KEYCODE_CALL = 5
     KEYCODE_ENDCALL = 6
     KEYCODE_0 = 7
@@ -374,121 +402,122 @@
 
     KEYCODE_LANGUAGE_SWITCH = 204
 
     KEYCODE_SLEEP = 223
     KEYCODE_WAKEUP = 224
 
     keys_map = {
-        '{LEFT}': KEYCODE_SOFT_LEFT,
-        '{RIGHT}': KEYCODE_SOFT_RIGHT,
-        '{HOME}': KEYCODE_HOME,
-        '{BACK}': KEYCODE_BACK,
-        '{MENU}': KEYCODE_MENU,
-        '{VOLUME_UP}': KEYCODE_VOLUME_UP,
-        '{VOLUME_DOWN}': KEYCODE_VOLUME_DOWN,
-        '{ENTER}': KEYCODE_ENTER,
-        '{BACKSPACE}': KEYCODE_DEL,
-        '{LEFT}': KEYCODE_DPAD_LEFT,
-        '{RIGHT}': KEYCODE_DPAD_RIGHT,
-        '{UP}': KEYCODE_DPAD_UP,
-        '{DOWN}': KEYCODE_DPAD_DOWN,
-        '{DEL}': KEYCODE_FORWARD_DEL,
-        '{DELETE}': KEYCODE_FORWARD_DEL,
-        '{POWER}': KEYCODE_POWER,
-        '{ESC}': KEYCODE_ESCAPE,
-        '`': KEYCODE_GRAVE,
-        '-': KEYCODE_MINUS,
-        '=': KEYCODE_EQUALS,
-        '[': KEYCODE_LEFT_BRACKET,
-        ']': KEYCODE_RIGHT_BRACKET,
-        '\\': KEYCODE_BACKSLASH,
-        ';': KEYCODE_SEMICOLON,
-        '\'': KEYCODE_APOSTROPHE,
-        '/': KEYCODE_SLASH,
-        '@': KEYCODE_AT,
-        '+': KEYCODE_PLUS,
-        ' ': KEYCODE_SPACE,
-        '\t': KEYCODE_TAB,
-        ',': KEYCODE_COMMA,
-        '.': KEYCODE_PERIOD
+        "{LEFT}": KEYCODE_SOFT_LEFT,
+        "{RIGHT}": KEYCODE_SOFT_RIGHT,
+        "{HOME}": KEYCODE_HOME,
+        "{BACK}": KEYCODE_BACK,
+        "{MENU}": KEYCODE_MENU,
+        "{VOLUME_UP}": KEYCODE_VOLUME_UP,
+        "{VOLUME_DOWN}": KEYCODE_VOLUME_DOWN,
+        "{ENTER}": KEYCODE_ENTER,
+        "{BACKSPACE}": KEYCODE_DEL,
+        "{LEFT}": KEYCODE_DPAD_LEFT,
+        "{RIGHT}": KEYCODE_DPAD_RIGHT,
+        "{UP}": KEYCODE_DPAD_UP,
+        "{DOWN}": KEYCODE_DPAD_DOWN,
+        "{DEL}": KEYCODE_FORWARD_DEL,
+        "{DELETE}": KEYCODE_FORWARD_DEL,
+        "{POWER}": KEYCODE_POWER,
+        "{ESC}": KEYCODE_ESCAPE,
+        "`": KEYCODE_GRAVE,
+        "-": KEYCODE_MINUS,
+        "=": KEYCODE_EQUALS,
+        "[": KEYCODE_LEFT_BRACKET,
+        "]": KEYCODE_RIGHT_BRACKET,
+        "\\": KEYCODE_BACKSLASH,
+        ";": KEYCODE_SEMICOLON,
+        "'": KEYCODE_APOSTROPHE,
+        "/": KEYCODE_SLASH,
+        "@": KEYCODE_AT,
+        "+": KEYCODE_PLUS,
+        " ": KEYCODE_SPACE,
+        "\t": KEYCODE_TAB,
+        ",": KEYCODE_COMMA,
+        ".": KEYCODE_PERIOD,
     }
 
     shift_chars = {
-        '~': '`',
-        '!': '1',
-        '#': '3',
-        '$': '4',
-        '%': '5',
-        '^': '6',
-        '&': '7',
-        '*': '8',
-        '(': '9',
-        ')': '0',
-        '_': '-',
-        '=': '+',
-        ':': ';',
+        "~": "`",
+        "!": "1",
+        "#": "3",
+        "$": "4",
+        "%": "5",
+        "^": "6",
+        "&": "7",
+        "*": "8",
+        "(": "9",
+        ")": "0",
+        "_": "-",
+        "=": "+",
+        ":": ";",
         '"': "'",
-        '<': ',',
-        '>': '.',
-        '?': '/'
+        "<": ",",
+        ">": ".",
+        "?": "/",
     }
 
     @staticmethod
     def get_key_list(text):
-        '''将字符串转换为按键列表
-        '''
+        """将字符串转换为按键列表"""
         i = 0
         result = []
         while i < len(text):
             asc = ord(text[i])
-            if asc >= ord('0') and asc <= ord('9'):
+            if asc >= ord("0") and asc <= ord("9"):
                 # 数字
-                result.append(KeyCode.KEYCODE_0 + asc - ord('0'))
-            elif asc >= ord('a') and asc <= ord('z'):
+                result.append(KeyCode.KEYCODE_0 + asc - ord("0"))
+            elif asc >= ord("a") and asc <= ord("z"):
                 # 小写字母
-                result.append(KeyCode.KEYCODE_A + asc - ord('a'))
-            elif asc >= ord('A') and asc <= ord('Z'):
+                result.append(KeyCode.KEYCODE_A + asc - ord("a"))
+            elif asc >= ord("A") and asc <= ord("Z"):
                 # 大写字母，加上SHIFT键
-                result.append([KeyCode.KEYCODE_SHIFT_LEFT, KeyCode.KEYCODE_A + asc - ord('A')])
-            elif asc == ord('{'):
+                result.append(
+                    [KeyCode.KEYCODE_SHIFT_LEFT, KeyCode.KEYCODE_A + asc - ord("A")]
+                )
+            elif asc == ord("{"):
                 # 自定义按键
-                end = text.find('}', i + 1)
+                end = text.find("}", i + 1)
                 if end < 0:
-                    raise RuntimeError('按键错误：%s' % text)
-                key = text[i:end + 1]
+                    raise RuntimeError("按键错误：%s" % text)
+                key = text[i : end + 1]
                 if key not in KeyCode.keys_map:
-                    raise RuntimeError('按键错误：%s' % key)
+                    raise RuntimeError("按键错误：%s" % key)
                 result.append(KeyCode.keys_map[key])
                 i = end
             elif text[i] in KeyCode.keys_map:
                 result.append(KeyCode.keys_map[text[i]])
             elif text[i] in KeyCode.shift_chars:
                 keys = KeyCode.get_key_list(KeyCode.shift_chars[text[i]])
                 keys.insert(0, KeyCode.KEYCODE_SHIFT_LEFT)
                 result.append(keys)
             else:
-                raise NotImplementedError('不支持的按键：%s' % text[i])
+                raise NotImplementedError("不支持的按键：%s" % text[i])
 
             i += 1
         return result
 
 
 class EnumThreadPriority(object):
-    '''线程优先级
-    '''
-    LOWEST = 'THREAD_PRIORITY_LOWEST'  # = 19
-    BACKGROUND = 'THREAD_PRIORITY_BACKGROUND'  # = 10
-    LESS_FAVORABLE = 'THREAD_PRIORITY_LESS_FAVORABLE'  # = +1
-    DEFAULT = 'THREAD_PRIORITY_DEFAULT'  # = 0
-    MORE_FAVORABLE = 'THREAD_PRIORITY_MORE_FAVORABLE'  # = -1
-    FOREGROUND = 'THREAD_PRIORITY_FOREGROUND'  # = -2
-    DISPLAY = 'THREAD_PRIORITY_DISPLAY'  # = -4
-    URGENT_DISPLAY = 'THREAD_PRIORITY_URGENT_DISPLAY'  # = -8
-    AUDIO = 'THREAD_PRIORITY_AUDIO'  # = -16
-    URGENT_AUDIO = 'THREAD_PRIORITY_URGENT_AUDIO'  # = -19
+    """线程优先级"""
+
+    LOWEST = "THREAD_PRIORITY_LOWEST"  # = 19
+    BACKGROUND = "THREAD_PRIORITY_BACKGROUND"  # = 10
+    LESS_FAVORABLE = "THREAD_PRIORITY_LESS_FAVORABLE"  # = +1
+    DEFAULT = "THREAD_PRIORITY_DEFAULT"  # = 0
+    MORE_FAVORABLE = "THREAD_PRIORITY_MORE_FAVORABLE"  # = -1
+    FOREGROUND = "THREAD_PRIORITY_FOREGROUND"  # = -2
+    DISPLAY = "THREAD_PRIORITY_DISPLAY"  # = -4
+    URGENT_DISPLAY = "THREAD_PRIORITY_URGENT_DISPLAY"  # = -8
+    AUDIO = "THREAD_PRIORITY_AUDIO"  # = -16
+    URGENT_AUDIO = "THREAD_PRIORITY_URGENT_AUDIO"  # = -19
 
 
 class ClassMethod(object):
     def __init__(self, method):
         self._method = method
 
     def __get__(self, instance, owner):
@@ -508,115 +537,123 @@
     def __init__(self, lock):
         self._lock = lock
 
     def __enter__(self):
         time_start = time.time()
         self._lock.acquire()
         time_delta = time.time() - time_start
-        if time_delta >= 0.1: logger.debug('thread %d wait %sS' % (threading.current_thread().ident, time_delta))
+        if time_delta >= 0.1:
+            logger.debug(
+                "thread %d wait %sS" % (threading.current_thread().ident, time_delta)
+            )
 
     def __exit__(self, type, value, traceback):
         self._lock.release()
 
 
 class ThreadEx(threading.Thread):
-    '''可以捕获异常的线程类
-    '''
+    """可以捕获异常的线程类"""
 
     def run(self):
-        '''重载run方法
-        '''
+        """重载run方法"""
         import platform
+
         if platform.system() == "Windows":
             try:
                 import pythoncom
             except ImportError:
                 pass
             else:
                 pythoncom.CoInitialize()
         try:
             return threading.Thread.run(self)
         except (KeyboardInterrupt, SystemExit):
             raise
         except:
             # sys.excepthook(*sys.exc_info())
-            logger.exception('thread %s exit' % self.getName())
+            logger.exception("thread %s exit" % self.getName())
 
 
 class Singleton(object):
-    '''单例基类
-    '''
+    """单例基类"""
+
     instance = None
 
     def __new__(cls, *args, **kwargs):
         if not cls.instance:
             cls.instance = super(Singleton, cls).__new__(cls, *args, **kwargs)
         return cls.instance
 
 
 def get_root_path():
-    '''获取根目录，支持py2exe打包后
-    '''
+    """获取根目录，支持py2exe打包后"""
     if hasattr(sys, "frozen"):
         # py2exe打包的
-        python_path = unicode(sys.executable, sys.getfilesystemencoding()) if six.PY2 else sys.executable
-        return os.path.join(os.path.dirname(python_path), 'library.zip')
-    file_path = unicode(eval('__file__'), sys.getfilesystemencoding()) if six.PY2 else eval('__file__')
+        python_path = (
+            unicode(sys.executable, sys.getfilesystemencoding())
+            if six.PY2
+            else sys.executable
+        )
+        return os.path.join(os.path.dirname(python_path), "library.zip")
+    file_path = (
+        unicode(eval("__file__"), sys.getfilesystemencoding())
+        if six.PY2
+        else eval("__file__")
+    )
     return os.path.dirname(file_path)
 
 
 def is_mutibyte_string(data):
-    '''判断是否是多字节字符串
-    '''
+    """判断是否是多字节字符串"""
     if six.PY2 and (not isinstance(data, unicode)):
-        data = data.decode('utf8')
+        data = data.decode("utf8")
     for c in data:
-        if ord(c) > 256: return True
+        if ord(c) > 256:
+            return True
     return False
 
 
 def get_string_hashcode(s):
-    '''计算java中String的hashcode值
-     * Returns a hash code for this string. The hash code for a
-     * <code>String</code> object is computed as
-     * <blockquote><pre>
-     * s[0]*31^(n-1) + s[1]*31^(n-2) + ... + s[n-1]
-     * </pre></blockquote>
-     * using <code>int</code> arithmetic, where <code>s[i]</code> is the
-     * <i>i</i>th character of the string, <code>n</code> is the length of
-     * the string, and <code>^</code> indicates exponentiation.
-     * (The hash value of the empty string is zero.)
-    '''
+    """计算java中String的hashcode值
+    * Returns a hash code for this string. The hash code for a
+    * <code>String</code> object is computed as
+    * <blockquote><pre>
+    * s[0]*31^(n-1) + s[1]*31^(n-2) + ... + s[n-1]
+    * </pre></blockquote>
+    * using <code>int</code> arithmetic, where <code>s[i]</code> is the
+    * <i>i</i>th character of the string, <code>n</code> is the length of
+    * the string, and <code>^</code> indicates exponentiation.
+    * (The hash value of the empty string is zero.)
+    """
     if six.PY2 and (not isinstance(s, unicode)):
-        s = s.decode('utf8')
+        s = s.decode("utf8")
     ret = 0
     max_val = 0x80000000
     for c in s:
         ret = ret * 31 + ord(c)
         ret %= max_val * 2
         if ret >= max_val:
             ret -= max_val * 2
     return ret
 
 
 def get_intersection(rect1, rect2):
-    '''计算两个区域的交集
-    '''
+    """计算两个区域的交集"""
     left = max(rect1[0], rect2[0])
     right = min(rect1[0] + rect1[2], rect2[0] + rect2[2])
     top = max(rect1[1], rect2[1])
     bottom = min(rect1[1] + rect1[3], rect2[1] + rect2[3])
     return (left, top, right - left, bottom - top)
 
 
 def get_process_name_hash(process_name, device_id):
-    '''根据进程名和设备id计算端口值
+    """根据进程名和设备id计算端口值
             结果范围：[5100, 5200)
     TODO: hash冲突的解决
-    '''
+    """
     result = 0
     start_port = 15000
     port_range = 1000
     text = device_id + process_name
     for i in range(len(text)):
         c = text[i]
         asc = ord(c)
@@ -624,124 +661,137 @@
 
     if result > port_range:
         result %= port_range
     return result + start_port
 
 
 def version_cmp(ver1, ver2):
-    '''版本比较
-    '''
-    if ver1 == ver2: return 0
-    ver1 = ver1.split('.')
-    ver2 = ver2.split('.')
+    """版本比较"""
+    if ver1 == ver2:
+        return 0
+    ver1 = ver1.split(".")
+    ver2 = ver2.split(".")
     i = 0
     while True:
-        if i >= len(ver1) and i >= len(ver2): return 0
-        if i >= len(ver1) and i < len(ver2): return -1
-        if i >= len(ver2) and i < len(ver1): return 1
+        if i >= len(ver1) and i >= len(ver2):
+            return 0
+        if i >= len(ver1) and i < len(ver2):
+            return -1
+        if i >= len(ver2) and i < len(ver1):
+            return 1
         if ver1[i].isdigit() and ver2[i].isdigit():
             c1 = int(ver1[i])
             c2 = int(ver2[i])
-            if c1 > c2: return 1
-            elif c1 < c2: return -1
+            if c1 > c2:
+                return 1
+            elif c1 < c2:
+                return -1
         elif ver1[i].isdigit():
             return 1
         elif ver2[i].isdigit():
             return -1
         else:
             return 0
         i += 1
 
 
 def list_zipfile_dir(zipfile_path, dir_path):
-    '''获取zip文件中指定目录的子目录和文件列表
-    '''
+    """获取zip文件中指定目录的子目录和文件列表"""
     import zipfile
+
     with zipfile.ZipFile(zipfile_path, "r") as z:
         result = []
         for it in z.namelist():
-            if it.startswith('%s/' % dir_path):
-                result.append(it[len(dir_path) + 1:])
+            if it.startswith("%s/" % dir_path):
+                result.append(it[len(dir_path) + 1 :])
         return result
 
 
 def extract_from_zipfile(zipfile_path, relative_path, save_path):
-    '''从zip文件中提取文件
-    '''
-    logger.info('extract_from_zipfile %s %s' % (relative_path, save_path))
+    """从zip文件中提取文件"""
+    logger.info("extract_from_zipfile %s %s" % (relative_path, save_path))
     import zipfile
+
     with zipfile.ZipFile(zipfile_path, "r") as z:
         try:
             z.getinfo(relative_path)
         except KeyError:
             for it in list_zipfile_dir(zipfile_path, relative_path):
-                extract_from_zipfile(zipfile_path, relative_path + '/' + it, os.path.join(save_path, it))
+                extract_from_zipfile(
+                    zipfile_path, relative_path + "/" + it, os.path.join(save_path, it)
+                )
         else:
             content = z.read(relative_path)
             save_dir = os.path.dirname(save_path)
             if not os.path.exists(save_dir):
                 os.makedirs(save_dir)
-            with open(save_path, 'wb') as f:
+            with open(save_path, "wb") as f:
                 f.write(content)
 
 
 def time_clock():
-    '''
-    '''
-    if sys.platform == 'win32':
+    """ """
+    if sys.platform == "win32":
         try:  # Python 3.4+
             return time.perf_counter()
         except AttributeError:  # Earlier than Python 3.
             return time.clock()
     else:
         return time.time()
-    
+
+
 def is_int(num):
-    '''判断整数num是否可以用32位表示
-    '''
-    return (num <= 2147483647 and num >= -2147483648)
+    """判断整数num是否可以用32位表示"""
+    return num <= 2147483647 and num >= -2147483648
+
 
 def general_encode(s):
-    '''字符串通用编码处理
+    """字符串通用编码处理
     python2 => utf8
     python3 => unicode
-    '''
+    """
     if six.PY2 and isinstance(s, (unicode,)):
-        s = s.encode('utf8')
+        s = s.encode("utf8")
     elif six.PY3 and isinstance(s, (bytes,)):
-        s = s.decode('utf8')
+        s = s.decode("utf8")
     return s
 
+
 def utf8_encode(s):
-    '''将字符串转换为utf8编码
-    '''
+    """将字符串转换为utf8编码"""
     if not isinstance(s, bytes):
-        s = s.encode('utf8')
+        s = s.encode("utf8")
     return s
-    
+
+
 def encode_wrap(func):
-    '''处理函数参数编码
-    '''
+    """处理函数参数编码"""
+
     def wrap_func(*args, **kwargs):
         args = list(args)
         for i, it in enumerate(args):
             args[i] = general_encode(it)
         for key in kwargs:
             kwargs[key] = general_encode(kwargs[key])
         return func(*args, **kwargs)
+
     return wrap_func
 
+
 def enforce_utf8_decode(s):
-    '''强制utf8解码，对于不合法的字符串，使用\x12的形式
-    '''
+    """强制utf8解码，对于不合法的字符串，使用\x12的形式"""
     if not isinstance(s, bytes):
         return s
     try:
-        return s.decode('utf8')
+        return s.decode("utf8")
     except UnicodeDecodeError as e:
         start = e.args[2]
         end = e.args[3]
-        return enforce_utf8_decode(s[:start]) + repr(s[start: end])[1:-1] + enforce_utf8_decode(s[end:])
+        return (
+            enforce_utf8_decode(s[:start])
+            + repr(s[start:end])[1:-1]
+            + enforce_utf8_decode(s[end:])
+        )
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     pass
```

### Comparing `qt4a-2.3.1/qt4a/androiddriver/webdriver.py` & `qt4a-3.0.0/qt4a/androiddriver/webdriver.py`

 * *Files identical despite different names*

### Comparing `qt4a-2.3.1/qt4a/androidtestbase.py` & `qt4a-3.0.0/qt4a/androidtestbase.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: UTF-8 -*-
 #
 # Tencent is pleased to support the open source community by making QTA available.
 # Copyright (C) 2016THL A29 Limited, a Tencent company. All rights reserved.
-# Licensed under the BSD 3-Clause License (the "License"); you may not use this 
+# Licensed under the BSD 3-Clause License (the "License"); you may not use this
 # file except in compliance with the License. You may obtain a copy of the License at
-# 
+#
 # https://opensource.org/licenses/BSD-3-Clause
-# 
-# Unless required by applicable law or agreed to in writing, software distributed 
+#
+# Unless required by applicable law or agreed to in writing, software distributed
 # under the License is distributed on an "AS IS" basis, WITHOUT WARRANTIES OR CONDITIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 #
 
-'''Android自动化测试基类
-'''
+"""Android自动化测试基类
+"""
 
 import sys, os, platform
 import time
 import re
 import shutil
 import tempfile
 import traceback
@@ -29,361 +29,462 @@
 from testbase.conf import settings
 from tuia.env import run_env, EnumEnvType
 
 from qt4a.androiddriver import util
 from qt4a.device import Device, DeviceProviderManager
 from qt4a.androidapp import AndroidApp
 
-util.set_default_encoding('utf8')  # 修改默认编码
- 
+util.set_default_encoding("utf8")  # 修改默认编码
+
+
 class EnumCrashType(object):
-    '''枚举crash类型
-    '''
+    """枚举crash类型
+    """
+
     NATIVE_SYSTEM_CRASH = "Native系统Crash"
-    NATIVE_NONE_SYSTEM_CRASH = "Native非系统Crash" 
+    NATIVE_NONE_SYSTEM_CRASH = "Native非系统Crash"
     JAVA_CRASH = "Java Crash"
     OTHER_CRASH = "其他类型Crash"
 
+
 def get_valid_file_name(file_name):
-    '''过滤掉文件名中的非法字符
-    '''
-    for c in (':', '?'):
-        file_name = file_name.replace(c, '_')
+    """过滤掉文件名中的非法字符
+    """
+    for c in (":", "?"):
+        file_name = file_name.replace(c, "_")
     return file_name
 
+
 class AndroidTestBase(tc.TestCase):
-    '''QT4A测试基类
-    '''
-    
+    """QT4A测试基类
+    """
+
     def init_test(self, testresult):
-        '''初始化测试环境。慎用此函数，尽量将初始化放到preTest里。
-        '''
+        """初始化测试环境。慎用此函数，尽量将初始化放到preTest里。
+        """
         super(AndroidTestBase, self).init_test(testresult)
         self._run_device = None
         self._target_crash_proc_list = []
         self._check_log_called = False
 
-    initTest = init_test   
-    
+    initTest = init_test
+
     def post_test(self):
-        '''清理测试用例
-        '''
+        """清理测试用例
+        """
         self._run_test_complete = True
-        if hasattr(self, '_record_thread_status_dict') and self._record_thread_status_dict:
+        if (
+            hasattr(self, "_record_thread_status_dict")
+            and self._record_thread_status_dict
+        ):
             timeout = 30
             time0 = time.time()
             while time.time() - time0 < timeout:
                 for key in self._record_thread_status_dict:
-                    if not self._record_thread_status_dict[key]: break
+                    if not self._record_thread_status_dict[key]:
+                        break
                 else:
                     break
                 time.sleep(0.1)
             else:
-                qta_logger.warn('wait for record screen thread exit timeout')
-            
+                qta_logger.warn("wait for record screen thread exit timeout")
+
         self._save_logcat()
         self._save_qt4a_log()
-        if hasattr(self, '_logcat_debug_level_list'):
+        if hasattr(self, "_logcat_debug_level_list"):
             for device in Device.device_list:
-                device_name = '%s' % device.device_id
+                device_name = "%s" % device.device_id
                 if device_name not in self._logcat_debug_level_list:
-                    msg = '设备:%s中的logcat没有debug级别的日志，请检查手机日志级别设置 ' % device_name
+                    msg = "设备:%s中的logcat没有debug级别的日志，请检查手机日志级别设置 " % device_name
                     if self._check_log_called:
                         qta_logger.error(msg)
                     else:
                         qta_logger.warn(msg)
 
-        if hasattr(settings, 'QT4A_DEVICE_HOSTS'):
+        if hasattr(settings, "QT4A_DEVICE_HOSTS"):
             for device in Device.device_list:
-                self.log_info('恢复设备: %s hosts环境' % device.device_id)
+                self.log_info("恢复设备: %s hosts环境" % device.device_id)
                 device.modify_hosts()
 
- 
     postTest = post_test
- 
+
     def clean_test(self):
-        '''清理测试环境。慎用此函数，尽量将清理放到postTest里。
-        '''
+        """清理测试环境。慎用此函数，尽量将清理放到postTest里。
+        """
         super(AndroidTestBase, self).clean_test()
         Device.release_all_device()  # 释放所有设备
 
     cleanTest = clean_test
 
     def acquire_device(self, device_id=None, **kwargs):
-        '''申请设备接口
+        """申请设备接口
         
         :param device_id: 设备ID，用于本地调试
         :type device_id:  string
-        '''
+        """
         if device_id:
-            kwargs['id'] = device_id
-        resource = self.test_resources.acquire_resource('android', condition=kwargs)
+            kwargs["id"] = device_id
+        resource = self.test_resources.acquire_resource("android", condition=kwargs)
+        util.logger.debug("Device info: %s" % resource)
         device = DeviceProviderManager().connect_device(resource)
-        if not device: raise RuntimeError('Connect device %s failed' % resource)
+        if not device:
+            raise RuntimeError("Connect device %s failed" % resource)
 
-        try:    
-            self.test_result.log_record(EnumLogLevel.Environment, '申请 %s 设备成功：%s(%s)' % ('Android', device.model, device.device_id), {"device":device.imei})
+        try:
+            self.test_result.log_record(
+                EnumLogLevel.Environment,
+                "申请 %s 设备成功：%s(%s)" % ("Android", device.model, device.device_id),
+                {"device": device.imei},
+            )
         except Exception as e:
-            qta_logger.warn('GetDeviceImei error:%s' % e)
+            qta_logger.warn("GetDeviceImei error:%s" % e)
 
-        if hasattr(settings, 'QT4A_DEVICE_HOSTS'):
+        if hasattr(settings, "QT4A_DEVICE_HOSTS"):
             device_hosts = settings.QT4A_DEVICE_HOSTS
             if device_hosts:
-                self.logInfo('设置设备hosts为：\n%s' % device_hosts)
+                self.logInfo("设置设备hosts为：\n%s" % device_hosts)
                 host_list = []
-                pattern = re.compile(r'\s*(\S+)\s+(\S+)\s*')
-                for line in device_hosts.split('\n'):
+                pattern = re.compile(r"\s*(\S+)\s+(\S+)\s*")
+                for line in device_hosts.split("\n"):
                     line = line.strip()
-                    if not line: continue
+                    if not line:
+                        continue
                     ret = pattern.match(line)
-                    if not ret: raise RuntimeError('hosts格式错误: %r' % line)
+                    if not ret:
+                        raise RuntimeError("hosts格式错误: %r" % line)
                     host_list.append((ret.group(1), ret.group(2)))
                 device.modify_hosts(host_list)
-            
+
         self.add_logcat_callback(device)
-        
-        if hasattr(settings, 'QT4A_RECORD_SCREEN') and settings.QT4A_RECORD_SCREEN == True:
-            if not hasattr(self, '_record_thread_status_dict'):
+
+        if (
+            hasattr(settings, "QT4A_RECORD_SCREEN")
+            and settings.QT4A_RECORD_SCREEN == True
+        ):
+            if not hasattr(self, "_record_thread_status_dict"):
                 self._record_thread_status_dict = {}
             self._record_thread_status_dict[device.device_id] = False
-            qta_logger.info('%s start record screen thread' % device.device_id)
-            t = util.ThreadEx(target=self._record_screen_thread, args=(device,), name='Device Record Screen Thread')
+            qta_logger.info("%s start record screen thread" % device.device_id)
+            t = util.ThreadEx(
+                target=self._record_screen_thread,
+                args=(device,),
+                name="Device Record Screen Thread",
+            )
             t.setDaemon(True)
             t.start()
         device.adb.start_logcat()
         return device
 
     def get_extra_fail_record(self):
-        '''用例执行失败时，用于获取用例相关的错误记录和附件信息
-        '''
-        from qt4a.androiddriver.util import logger as qt4a_logger
+        """用例执行失败时，用于获取用例相关的错误记录和附件信息
+        """
         pic_attachments = {}
         for device in Device.device_list:
-            pic_path = "%s_%s_%s.png" % (self.__class__.__name__, get_valid_file_name(device.device_id), time.time())
+            pic_path = "%s_%s_%s.png" % (
+                self.__class__.__name__,
+                get_valid_file_name(device.device_id),
+                time.time(),
+            )
             try:
                 device.take_screen_shot(pic_path)
                 if os.path.isfile(pic_path):
-                    pic_attachments['%s的截图' % device.device_id] = pic_path
+                    pic_attachments["%s的截图" % device.device_id] = pic_path
                 else:
-                    qt4a_logger.error('pic %s not exist' % pic_path)
+                    util.logger.error("pic %s not exist" % pic_path)
             except Exception as e:
-                qt4a_logger.error('take_screen_shot error: %s' % e)
-                qt4a_logger.error(''.join(traceback.format_tb(sys.exc_info()[2])))
+                util.logger.error("take_screen_shot error: %s" % e)
+                util.logger.error("".join(traceback.format_tb(sys.exc_info()[2])))
         return {}, pic_attachments
 
     def take_screen_shot(self, app_or_device, info):
-        '''生成当前指定设备的屏幕截图
+        """生成当前指定设备的屏幕截图
         
         :param app: AndroidApp类或AndroidDevice实例
         :type app:  AndroidApp or AndroidDevice
         :param info: 显示的提示信息
         :type info:  string
-        '''
-        
+        """
+
         device = app_or_device
         if isinstance(app_or_device, AndroidApp):
             device = app_or_device.device
-        path = self.__class__.__name__ + '_' + get_valid_file_name(device.device_id) + '_' + str(int(time.time())) + '.jpg'
+        path = (
+            self.__class__.__name__
+            + "_"
+            + get_valid_file_name(device.device_id)
+            + "_"
+            + str(int(time.time()))
+            + ".jpg"
+        )
         device.take_screen_shot(path)
-        self.test_result.info(info, attachments={'截图':path})
-    
+        self.test_result.info(info, attachments={"截图": path})
+
     def _record_screen_thread(self, device):
-        '''录屏线程
-        '''
+        """录屏线程
+        """
         from qt4a.androiddriver.devicedriver import qt4a_path
+
         record_time = 4 * 1000  # 每次录制的时间
         framerate = 8
         quality = 20
-        remote_tmp_path_tmpl = '%s/screen.record.%%d' % qt4a_path
+        remote_tmp_path_tmpl = "%s/screen.record.%%d" % qt4a_path
         max_record_file_count = 4  # 最大临时存储的录屏文件数目
         index = 0
-        device.delete_file('%s/screen.record.*' % qt4a_path)
-        
-        while not hasattr(self, '_run_test_complete') or self._run_test_complete == False:
+        device.delete_file("%s/screen.record.*" % qt4a_path)
+
+        while (
+            not hasattr(self, "_run_test_complete") or self._run_test_complete == False
+        ):
             # 尚未结束
             remote_tmp_path = remote_tmp_path_tmpl % (index % max_record_file_count)
-            device.run_shell_cmd('%s/screenshot record -p %s -t %d -f %d -q %d' % (qt4a_path, remote_tmp_path, record_time, framerate, quality))
+            device.run_shell_cmd(
+                "%s/screenshot record -p %s -t %d -f %d -q %d"
+                % (qt4a_path, remote_tmp_path, record_time, framerate, quality)
+            )
             index += 1
-            if index >= max_record_file_count: index -= max_record_file_count
-            
+            if index >= max_record_file_count:
+                index -= max_record_file_count
+
         if not self.test_result.passed:
             merge_file_list = []
             for i in range(max_record_file_count):
-                merge_file_list.append(remote_tmp_path_tmpl % ((i + index) % max_record_file_count))
-            device.run_shell_cmd('cat %s > %s' % (' '.join(merge_file_list), remote_tmp_path_tmpl % max_record_file_count))
-            local_tmp_path = tempfile.mktemp('.record')
-            device.pull_file(remote_tmp_path_tmpl % max_record_file_count, local_tmp_path)
-            save_dir = tempfile.mkdtemp('.screenshot')
+                merge_file_list.append(
+                    remote_tmp_path_tmpl % ((i + index) % max_record_file_count)
+                )
+            device.run_shell_cmd(
+                "cat %s > %s"
+                % (
+                    " ".join(merge_file_list),
+                    remote_tmp_path_tmpl % max_record_file_count,
+                )
+            )
+            local_tmp_path = tempfile.mktemp(".record")
+            device.pull_file(
+                remote_tmp_path_tmpl % max_record_file_count, local_tmp_path
+            )
+            save_dir = tempfile.mkdtemp(".screenshot")
             frame_list = Device.extract_record_frame(local_tmp_path, save_dir)
-            video_path = self.__class__.__name__ + '_' + get_valid_file_name(device.device_id) + '_' + str(int(time.time())) + '.mp4'
+            video_path = (
+                self.__class__.__name__
+                + "_"
+                + get_valid_file_name(device.device_id)
+                + "_"
+                + str(int(time.time()))
+                + ".mp4"
+            )
             result = Device.screen_frame_to_video(frame_list, framerate, video_path)
             if result == None:
-                qta_logger.warn('opencv not installed')
+                qta_logger.warn("opencv not installed")
             else:
-                self.test_result.info('最近15秒录屏', attachments={video_path: video_path})
+                self.test_result.info("最近15秒录屏", attachments={video_path: video_path})
             shutil.rmtree(save_dir)
-        
+
         self._record_thread_status_dict[device.device_id] = True
-        
+
     def _save_qt4a_log(self):
-        '''保存QT4A日志
-        '''
-        if run_env == EnumEnvType.Lab or (hasattr(settings, 'QT4A_UPLOAD_QT4A_LOG') and settings.QT4A_UPLOAD_QT4A_LOG == True):
-            filename = 'qt4a_%s_%s.log' % (self.__class__.__name__, int(time.time()))
+        """保存QT4A日志
+        """
+        if run_env == EnumEnvType.Lab or (
+            hasattr(settings, "QT4A_UPLOAD_QT4A_LOG")
+            and settings.QT4A_UPLOAD_QT4A_LOG == True
+        ):
+            filename = "qt4a_%s_%s.log" % (self.__class__.__name__, int(time.time()))
             shutil.copyfile(util.logger_path, filename)
-            self.test_result.info('QT4A日志', attachments={filename: filename})
+            self.test_result.info("QT4A日志", attachments={filename: filename})
             util.clear_logger_file()
-            
+
     def _save_logcat(self):
-        '''保存logcat日志
-        '''
+        """保存logcat日志
+        """
         crash_files = {}
         logcat_files = {}
-        crash_type = ''
+        crash_type = ""
         for device in Device.device_list:
             device.adb.stop_logcat()
-            ret_type, crash_path = self.extract_crash_from_logcat(device.adb.get_log(False))
-            devicename = '设备:%s' % device.device_id
+            ret_type, crash_path = self.extract_crash_from_logcat(
+                device.adb.get_log(False)
+            )
+            devicename = "设备:%s" % device.device_id
             if crash_path:
                 crash_type = ret_type
                 crash_files[devicename] = crash_path
-            log_path = '%s_%s_%s.log' % (self.__class__.__name__, get_valid_file_name(device.device_id), int(time.time()))
+            log_path = "%s_%s_%s.log" % (
+                self.__class__.__name__,
+                get_valid_file_name(device.device_id),
+                int(time.time()),
+            )
             device.adb.save_log(log_path)
             if os.path.isfile(log_path):
                 logcat_files[devicename] = log_path
             else:
-                self.test_result.warning('保存logcat文件: %s失败' % log_path)
-                      
-        if logcat_files: 
-            if not self.test_result.passed or crash_files or (hasattr(settings, 'UPLOAD_LOGCAT_WHEN_PASS') and settings.UPLOAD_LOGCAT_WHEN_PASS):
+                self.test_result.warning("保存logcat文件: %s失败" % log_path)
+
+        if logcat_files:
+            if (
+                not self.test_result.passed
+                or crash_files
+                or (
+                    hasattr(settings, "UPLOAD_LOGCAT_WHEN_PASS")
+                    and settings.UPLOAD_LOGCAT_WHEN_PASS
+                )
+            ):
                 try:
-                    self.test_result.info('logcat日志', attachments=logcat_files)
+                    self.test_result.info("logcat日志", attachments=logcat_files)
                 except:
-                    qta_logger.exception('上传logcat文件[%s]失败' % logcat_files)
+                    qta_logger.exception("上传logcat文件[%s]失败" % logcat_files)
 
         if crash_files:
-            crash_title = "系统Crash(可不提单)：" if crash_type == EnumCrashType.NATIVE_SYSTEM_CRASH else "App Crash错误报告："
-            self.test_result.log_record(EnumLogLevel.APPCRASH, crash_title, attachments=crash_files)
+            crash_title = (
+                "系统Crash(可不提单)："
+                if crash_type == EnumCrashType.NATIVE_SYSTEM_CRASH
+                else "App Crash错误报告："
+            )
+            self.test_result.log_record(
+                EnumLogLevel.APPCRASH, crash_title, attachments=crash_files
+            )
 
     def extract_crash_from_logcat(self, log_list):
-        '''检测logcat日志中是否有crash发生并萃取出相关日志
-        '''
+        """检测logcat日志中是否有crash发生并萃取出相关日志
+        """
         from qt4a.androiddriver.util import logger as qt4a_logger
+
         pattern_list = self.extract_crash_by_patterns()
         if self._target_crash_proc_list == []:  # 表示用户不关心任何进程的crash问题，则不对crash进行提取
             return None, None
-        
-        if not isinstance(pattern_list, list) and not isinstance(pattern_list, tuple) and not len(pattern_list) == 2:
-            raise RuntimeError('传入的pattern_list不是列表或二元组')
+
+        if (
+            not isinstance(pattern_list, list)
+            and not isinstance(pattern_list, tuple)
+            and not len(pattern_list) == 2
+        ):
+            raise RuntimeError("传入的pattern_list不是列表或二元组")
         if isinstance(pattern_list, tuple):
             pattern_list = [pattern_list]
-        
+
         new_pattern_list = []
         for proc in self._target_crash_proc_list:
             if not isinstance(proc, str):
-                qt4a_logger.warn('传入的process不是字符串类型')
+                qt4a_logger.warn("传入的process不是字符串类型")
                 continue
             for pattern in pattern_list:
                 if not isinstance(pattern, tuple) or not len(pattern) == 2:
-                    qt4a_logger.warn('传入的pattern不是二元组')
+                    qt4a_logger.warn("传入的pattern不是二元组")
                 else:
-                    new_pattern_list.append((proc,) + pattern)  
-            new_pattern_list.append((proc,) + (r'AndroidRuntime', r'FATAL EXCEPTION:.*'))  # system crash1:java crash
-            # new_pattern_list.append((proc,) + (r'dalvikvm', r'threadid=.*: thread exiting with uncaught exception .*')) #与system crash1重复，暂时注释掉,优先取system crash1   
-            native_crash_pattern = r'pid: \d+, tid: \d+, name: .*>>> ' + '(' + proc + ')' + r' <<<'
-            new_pattern_list.append((r'/system/bin/debuggerd', r'DEBUG', native_crash_pattern))  # system crash2:native crash
+                    new_pattern_list.append((proc,) + pattern)
+            new_pattern_list.append(
+                (proc,) + (r"AndroidRuntime", r"FATAL EXCEPTION:.*")
+            )  # system crash1:java crash
+            # new_pattern_list.append((proc,) + (r'dalvikvm', r'threadid=.*: thread exiting with uncaught exception .*')) #与system crash1重复，暂时注释掉,优先取system crash1
+            native_crash_pattern = (
+                r"pid: \d+, tid: \d+, name: .*>>> " + "(" + proc + ")" + r" <<<"
+            )
+            new_pattern_list.append(
+                (r"/system/bin/debuggerd", r"DEBUG", native_crash_pattern)
+            )  # system crash2:native crash
         # new_pattern_list.append((r'/system/bin/debuggerd', r'DEBUG', r'signal \d+ \(.*\), code \d+ \(.*\), fault addr.*')) #fault addr crash与上一行的system crash2重复，优先取system crash2
-        
+
         if new_pattern_list == []:  # 因为可能随着需求变更，没有规则写入
             return None, None
-        
-        crash_info = ''
-        pattern = r'\[(.*)\(\d+\)\] \[.*\] (.)/(.*)\((\d+)\): (.*)'
+
+        crash_info = ""
+        pattern = r"\[(.*)\(\d+\)\] \[.*\] (.)/(.*)\((\d+)\): (.*)"
         form_log_dict = {}
-        regex = re.compile(pattern)        
+        regex = re.compile(pattern)
         for log in log_list:
             res = regex.match(log)
             if res:
-                cur_line = {'process_name': res.group(1), 'level': res.group(2), 'tag':res.group(3), 'part_log': res.group(5), 'line_log': log}  # res.group(1)是进程名process_name的正则表达式，res.group(2)是错误级别level的正则表达式，res.group(3)是标签tag的正则表达式，res.group(4)是线程id的正则表达式，res.group(5)是线程id后的冒号后开始到本行结尾内容的正则表达式，line_log存储整行日志log。
+                cur_line = {
+                    "process_name": res.group(1),
+                    "level": res.group(2),
+                    "tag": res.group(3),
+                    "part_log": res.group(5),
+                    "line_log": log,
+                }  # res.group(1)是进程名process_name的正则表达式，res.group(2)是错误级别level的正则表达式，res.group(3)是标签tag的正则表达式，res.group(4)是线程id的正则表达式，res.group(5)是线程id后的冒号后开始到本行结尾内容的正则表达式，line_log存储整行日志log。
                 if res.group(4) in form_log_dict:
                     form_log_dict[res.group(4)].append(cur_line)
                 else:
                     form_log_dict[res.group(4)] = [cur_line]
             else:
                 qt4a_logger.warn("提取crash日志时，log:%s无法按格式%s解析" % (log, pattern))
         crash_list = []
         for tlog_list in form_log_dict.values():
             is_crashed = False
-            tag = ''
+            tag = ""
             last_pattern_list = []
             for tlog_dict in tlog_list:
-                if is_crashed == True and tag == tlog_dict['tag']:
-                    crash_info += tlog_dict['line_log'] + '\n'  
+                if is_crashed == True and tag == tlog_dict["tag"]:
+                    crash_info += tlog_dict["line_log"] + "\n"
                     crash_list.append(tlog_dict)
                     continue
                 if not last_pattern_list:
                     for pat_tuple in new_pattern_list:
                         process_name_reg = re.compile(pat_tuple[0])
-                        if not process_name_reg.match(tlog_list[0]['process_name']):
+                        if not process_name_reg.match(tlog_list[0]["process_name"]):
                             continue
                         last_pattern_list.append(pat_tuple)
                     if len(last_pattern_list) == 0:
                         break
-                is_crashed = False    
+                is_crashed = False
                 for pat_tuple in last_pattern_list:
                     tag_reg = re.compile(pat_tuple[1])
-                    tag = tlog_dict['tag']
+                    tag = tlog_dict["tag"]
                     if not tag_reg.match(tag):
                         continue
                     part_log_reg = re.compile(pat_tuple[2])
-                    if not part_log_reg.match(tlog_dict['part_log']):
+                    if not part_log_reg.match(tlog_dict["part_log"]):
                         continue
                     is_crashed = True
                     crash_list.append(tlog_dict)
-                    crash_info += tlog_dict['line_log'] + '\n'  
+                    crash_info += tlog_dict["line_log"] + "\n"
                     break
         if crash_info:
             crash_type = self.check_crash_type(crash_list)
-            crash_path = '%s_%s.crash.log' % (self.__class__.__name__, int(time.time()))
-            with open(crash_path, 'w') as fd:
+            crash_path = "%s_%s.crash.log" % (self.__class__.__name__, int(time.time()))
+            with open(crash_path, "w") as fd:
                 fd.write(crash_info)
             return crash_type, crash_path
         return None, None
-    
-    def check_crash_type(self, crash_list): 
+
+    def check_crash_type(self, crash_list):
         system_so_cnt = 3
         match_backtrace_begin = False
         # system_crash_demo:#01  pc 0002eed0  /system/lib/libgui.so (_ZN7android7Surface11queueBufferEP19ANativeWindowBufferi)
-        system_crash_pattern = r'#\d{2}  pc \w{8}  (/system/lib/.*\.so|/system/vendor/.*\.so)($| \(.*\))'
+        system_crash_pattern = (
+            r"#\d{2}  pc \w{8}  (/system/lib/.*\.so|/system/vendor/.*\.so)($| \(.*\))"
+        )
         system_crash_reg = re.compile(system_crash_pattern)
         system_so_set = set([])
         for tlog_dict in crash_list:
-            if tlog_dict['tag'] == 'native_eup':
-                res = system_crash_reg.match(tlog_dict['part_log'])
+            if tlog_dict["tag"] == "native_eup":
+                res = system_crash_reg.match(tlog_dict["part_log"])
                 if match_backtrace_begin and res:
                     system_so_set.add(res.group(1))
                     if len(system_so_set) == system_so_cnt:
-                        return EnumCrashType.NATIVE_SYSTEM_CRASH                    
-                elif tlog_dict['part_log'] == 'unwind_backtrace_with_ptrace start':
+                        return EnumCrashType.NATIVE_SYSTEM_CRASH
+                elif tlog_dict["part_log"] == "unwind_backtrace_with_ptrace start":
                     match_backtrace_begin = True
-                elif 'unwinded end stack_depth' in tlog_dict['part_log']:
-                    match_backtrace_begin = False  
-                    system_so_set = set([])              
+                elif "unwinded end stack_depth" in tlog_dict["part_log"]:
+                    match_backtrace_begin = False
+                    system_so_set = set([])
         return EnumCrashType.OTHER_CRASH
 
     def extract_crash_by_patterns(self):
         return None
-    
+
     def add_logcat_callback(self, device):
-        '''判断logcat日志中是否包含debug级别的日志，如果没有，很有可能该手机可以设置日志级别，且本身已设置了过滤debug级别的日志,可尝试操作手机设置
-        '''
-        if not hasattr(self, '_logcat_debug_level_list'):self._logcat_debug_level_list = []
+        """判断logcat日志中是否包含debug级别的日志，如果没有，很有可能该手机可以设置日志级别，且本身已设置了过滤debug级别的日志,可尝试操作手机设置
+        """
+        if not hasattr(self, "_logcat_debug_level_list"):
+            self._logcat_debug_level_list = []
+
         def wrap_func(pid, process_name, date, timestamp, level, tag, tid, content):
-            device_name = '%s' % device.device_id
+            device_name = "%s" % device.device_id
             if device_name in self._logcat_debug_level_list:
                 return
-            if level in ['D', 'V']:
+            if level in ["D", "V"]:
                 self._logcat_debug_level_list.append(device_name)
+
         device.adb.add_logcat_callback(wrap_func)
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     pass
```

### Comparing `qt4a-2.3.1/qt4a/apktool/__init__.py` & `qt4a-3.0.0/qt4a/apktool/__init__.py`

 * *Files identical despite different names*

### Comparing `qt4a-2.3.1/qt4a/apktool/apkfile.py` & `qt4a-3.0.0/qt4a/apktool/apkfile.py`

 * *Files identical despite different names*

### Comparing `qt4a-2.3.1/qt4a/apktool/axml.py` & `qt4a-3.0.0/qt4a/apktool/axml.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,19 +94,21 @@
     COMPATIBLE_WIDTH_LIMIT_DP_ATTR = 0x01010365
     LARGEST_WIDTH_LIMIT_DP_ATTR = 0x01010366
     STOP_WITH_TASK_ATTR = 'stopWithTask', 0x101036a
     PUBLIC_KEY_ATTR = 0x010103a6
     ISOLATED_PROCESS = 'isolatedProcess', 0x10103a9
     SUPPORTS_RT1 = 'supportsRtl', 0x10103af
     CATEGORY_ATTR = 0x010103e8
+    USES_CLEARTEXT_TRAFFIC_ATTR = 'usesCleartextTraffic', 0x10104ec
     RESIZEABLE_ACTIVITY_ATTR = 'resizeableActivity', 0x10104f6
     NETWORK_SECURITY_CONFIG = 'networkSecurityConfig', 0x1010527
     COMPILE_SDK_VERSION_ATTR = 'compileSdkVersion', 0x01010572
     COMPILE_SDK_VERSION_CODENAME_ATTR = 'compileSdkVersionCodename', 0x01010573
     APP_COMPONENTFACTORY = 'appComponentFactory', 0x101057a
+    FOREGROUND_SERVICE_TYPE_ATTR = 'foregroundServiceType', 0x1010599
 
     @staticmethod
     def list():
         '''获取attr列表
         '''
         result = []
         for key in EnumAttrType.__dict__:
```

### Comparing `qt4a-2.3.1/qt4a/apktool/header.py` & `qt4a-3.0.0/qt4a/apktool/header.py`

 * *Files identical despite different names*

### Comparing `qt4a-2.3.1/qt4a/apktool/manifest.py` & `qt4a-3.0.0/qt4a/apktool/manifest.py`

 * *Files identical despite different names*

### Comparing `qt4a-2.3.1/qt4a/apktool/repack.py` & `qt4a-3.0.0/qt4a/apktool/repack.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,299 +9,351 @@
 #
 # Unless required by applicable law or agreed to in writing, software distributed
 # under the License is distributed on an "AS IS" basis, WITHOUT WARRANTIES OR CONDITIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 #
 
-'''重打包
-'''
+"""重打包
+"""
 
-import six
 import json
 import logging
 import os
-import shutil
 import sys
 import subprocess
 import tempfile
+
 from qt4a.apktool.apkfile import APKFile
 from qt4a.apktool.manifest import AndroidManifest
 
 
 class MergeDexError(RuntimeError):
-    '''合并dex失败错误
-    '''
+    """合并dex失败错误
+    """
+
     pass
 
 
 class TooManyMethodsError(MergeDexError):
-    '''方法数超标
-    '''
+    """方法数超标
+    """
+
     pass
 
 
 class OutOfMemoryError(RuntimeError):
-    '''内存超标
-    '''
+    """内存超标
+    """
+
     pass
 
 
 def general_decode(s):
     if not isinstance(s, bytes):
         return s
     try:
-        return s.decode('utf8')
-    except:
-        return s.decode('gbk')
+        return s.decode("utf8")
+    except UnicodeDecodeError:
+        return s.decode("gbk")
 
 
 def get_apk_signature(rsa_file_path):
-    '''获取应用签名
-    '''
+    """获取应用签名
+    """
     if not os.path.exists(rsa_file_path):
-        raise RuntimeError('Rsa file %s not exist' % rsa_file_path)
+        raise RuntimeError("Rsa file %s not exist" % rsa_file_path)
     cur_path = os.path.dirname(os.path.abspath(__file__))
-    jar_path = os.path.join(cur_path, 'tools', 'apkhelper.jar')
-    return os.popen('java -jar %s getSignature %s' % (jar_path, rsa_file_path)).read()
+    jar_path = os.path.join(cur_path, "tools", "apkhelper.jar")
+    return os.popen("java -jar %s getSignature %s" % (jar_path, rsa_file_path)).read()
 
 
 def dex2jar(dex_path, jar_path):
-    '''将dex转换为jar
-    '''
+    """将dex转换为jar
+    """
     if not os.path.exists(dex_path):
-        raise RuntimeError('dex %s not exist' % dex_path)
+        raise RuntimeError("dex %s not exist" % dex_path)
     cur_path = os.path.dirname(os.path.abspath(__file__))
-    tools_path = os.path.join(cur_path, 'tools')
+    tools_path = os.path.join(cur_path, "tools")
     class_paths = []
     for it in os.listdir(tools_path):
-        if it.endswith('.jar'):
+        if it.endswith(".jar"):
             class_paths.append(os.path.join(tools_path, it))
     # -Xms512m -Xmx1024m
-    sep = ';' if sys.platform == 'win32' else ':'
-    cmdline = ['java', '-Xmx1024m', '-cp', sep.join(class_paths), 'com.googlecode.dex2jar.tools.Dex2jarCmd',
-               '-f', '-o', jar_path, dex_path]
-    logging.info(' '.join(cmdline))
-    proc = subprocess.Popen(
-        cmdline, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+    sep = ";" if sys.platform == "win32" else ":"
+    cmdline = [
+        "java",
+        "-Xmx1024m",
+        "-cp",
+        sep.join(class_paths),
+        "com.googlecode.dex2jar.tools.Dex2jarCmd",
+        "-f",
+        "-o",
+        jar_path,
+        dex_path,
+    ]
+    logging.info(" ".join(cmdline))
+    proc = subprocess.Popen(cmdline, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
     result = proc.communicate()[1]
-    if not b'->' in result:
-        raise RuntimeError('convert dex %s to jar failed: %s' %
-                           (dex_path, result))
+    if b"->" not in result:
+        raise RuntimeError("convert dex %s to jar failed: %s" % (dex_path, result))
 
 
 def jar2dex(jar_path, dex_path, max_heap_size=0):
-    '''jar转换为dex
-    '''
+    """jar转换为dex
+    """
     if not os.path.exists(jar_path):
-        raise RuntimeError('jar %s not exist' % jar_path)
+        raise RuntimeError("jar %s not exist" % jar_path)
     cur_path = os.path.dirname(os.path.abspath(__file__))
-    dx_path = os.path.join(cur_path, 'tools', 'dx.jar')
+    dx_path = os.path.join(cur_path, "tools", "dx.jar")
     # cmdline = 'java -Xmx1024m -cp "%s" com.android.dx.command.Main --dex --force-jumbo --output="%s" "%s"' % (dx_path, dex_path, jar_path)
     memory = 1024
     if max_heap_size:
         memory = max_heap_size
     elif os.path.getsize(jar_path) >= 8 * 1024 * 1024:
         memory = 2048  # 此时必须用64位java
-    cmdline = ['java', '-Xmx%dm' % memory, '-cp', dx_path, 'com.android.dx.command.Main',
-               '--dex', '--force-jumbo', '--output=%s' % dex_path, jar_path]
-    logging.info(' '.join(cmdline))
+    cmdline = [
+        "java",
+        "-Xmx%dm" % memory,
+        "-cp",
+        dx_path,
+        "com.android.dx.command.Main",
+        "--dex",
+        "--force-jumbo",
+        "--output=%s" % dex_path,
+        jar_path,
+    ]
+    logging.info(" ".join(cmdline))
 
-    proc = subprocess.Popen(
-        cmdline, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+    proc = subprocess.Popen(cmdline, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
     result = proc.communicate()[1]
     if result:
         err_msg = result
-        if sys.platform == 'win32':
-            err_msg = err_msg.decode('gbk')
+        if sys.platform == "win32":
+            err_msg = err_msg.decode("gbk")
         else:
-            err_msg = err_msg.decode('utf8')
+            err_msg = err_msg.decode("utf8")
         if proc.returncode:
-            if 'java.lang.OutOfMemoryError' in err_msg:
+            if "java.lang.OutOfMemoryError" in err_msg:
                 raise OutOfMemoryError(err_msg)
             else:
                 raise RuntimeError(
-                    'Convert jar %s to dex failed: %s' % (jar_path, err_msg))
+                    "Convert jar %s to dex failed: %s" % (jar_path, err_msg)
+                )
         else:
             logging.warning(err_msg)
 
 
 def rebuild_dex_with_jumbo(dex_path, max_heap_size=0):
-    '''使用jumbo模式重新编译dex
-    '''
-    jar_path = tempfile.mktemp('.jar')
+    """使用jumbo模式重新编译dex
+    """
+    jar_path = tempfile.mktemp(".jar")
     dex2jar(dex_path, jar_path)
     jar2dex(jar_path, dex_path, max_heap_size)
     os.remove(jar_path)
 
 
 def merge_dex(dst_dex, src_dexs, max_heap_size=0):
-    '''合并dex
-    '''
+    """合并dex
+    """
     cur_path = os.path.dirname(os.path.abspath(__file__))
-    jar_path = os.path.join(cur_path, 'tools', 'apkhelper.jar')
-    cmdline = ['java', '-jar', jar_path, 'mergeDex', dst_dex]
+    jar_path = os.path.join(cur_path, "tools", "apkhelper.jar")
+    cmdline = ["java", "-jar", jar_path, "mergeDex", dst_dex]
     cmdline.extend(src_dexs)
-    logging.info(' '.join(cmdline))
-    proc = subprocess.Popen(
-        cmdline, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+    logging.info(" ".join(cmdline))
+    proc = subprocess.Popen(cmdline, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
     result = proc.communicate()
-    if not b'Took' in result[0]:
-        if b'non-jumbo instruction' in result[1]:
+    if b"Took" not in result[0]:
+        if b"non-jumbo instruction" in result[1]:
             # 应用未使用jumbo模式编译，这里做一次转换
-            logging.warn('change dex to jumbo mode')
+            logging.warn("change dex to jumbo mode")
             rebuild_dex_with_jumbo(src_dexs[0], max_heap_size)
             return merge_dex(dst_dex, src_dexs, max_heap_size)
-        elif b'DexIndexOverflowException' in result[1]:
-            raise TooManyMethodsError('Merge dex failed: %s' % result[1])
+        elif b"DexIndexOverflowException" in result[1]:
+            raise TooManyMethodsError("Merge dex failed: %s" % result[1])
         else:
-            raise MergeDexError('Merge dex failed: %s' % result[1])
+            raise MergeDexError("Merge dex failed: %s" % result[1])
 
 
 def resign_apk(apk_path):
-    '''重签名应用
-    '''
+    """重签名应用
+    """
     if not os.path.exists(apk_path):
-        raise RuntimeError('apk %s not exist' % apk_path)
+        raise RuntimeError("apk %s not exist" % apk_path)
     cur_path = os.path.dirname(os.path.abspath(__file__))
-    key_file_path = os.path.join(cur_path, 'tools', 'qt4a.keystore')
-    save_path = apk_path[:-4] + '-signed.apk'
+    key_file_path = os.path.join(cur_path, "tools", "qt4a.keystore")
+    save_path = apk_path[:-4] + "-signed.apk"
     # 'jarsigner -digestalg SHA1 -sigalg MD5withRSA -keystore %s -signedjar %s %s qt4a' % (key_file_path, save_path, apk_path)
-    cmdline = ['jarsigner', '-digestalg', 'SHA1', '-sigalg', 'MD5withRSA', '-keystore',
-               key_file_path, '-signedjar', save_path, apk_path, 'qt4a']
-    logging.info(' '.join(cmdline))
-    proc = subprocess.Popen(cmdline, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
-    out, err = proc.communicate(b'test@123')
+    cmdline = [
+        "jarsigner",
+        "-digestalg",
+        "SHA1",
+        "-sigalg",
+        "MD5withRSA",
+        "-keystore",
+        key_file_path,
+        "-signedjar",
+        save_path,
+        apk_path,
+        "qt4a",
+    ]
+    logging.info(" ".join(cmdline))
+    proc = subprocess.Popen(
+        cmdline, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.PIPE
+    )
+    out, err = proc.communicate(b"test@123")
     if out:
-        logging.info('jarsigner: ' + general_decode(out))
+        logging.info("jarsigner: " + general_decode(out))
     if err:
-        logging.warn('jarsigner: ' + general_decode(err))
+        logging.warn("jarsigner: " + general_decode(err))
     return save_path
 
 
-def repack_apk(apk_path_or_list, provider_name, merge_dex_path, activity_list=None, res_file_list=None, debuggable=None, vm_safe_mode=None, max_heap_size=0, force_append=False):
-    '''
-    '''
+def repack_apk(
+    apk_path_or_list,
+    provider_name,
+    merge_dex_path,
+    activity_list=None,
+    res_file_list=None,
+    debuggable=None,
+    vm_safe_mode=None,
+    max_heap_size=0,
+    force_append=False,
+):
+    """
+    """
     if not isinstance(apk_path_or_list, list):
         apk_path_or_list = [apk_path_or_list]
     elif len(apk_path_or_list) == 0:
-        raise ValueError('apk path not specified')
+        raise ValueError("apk path not specified")
 
     apk_file_list = []
     signature_dict = {}
+    max_child_process = 38
     for it in apk_path_or_list:
         apk_file = APKFile(it)
         apk_file_list.append(apk_file)
         manifest = AndroidManifest(apk_file)
-        if debuggable != None:
+        if debuggable is not None:
             manifest.debuggable = debuggable  # 修改debuggable属性
-        if vm_safe_mode != None:
+        if vm_safe_mode is not None:
             manifest.vm_safe_mode = vm_safe_mode  # 修改安全模式
+        if manifest.min_sdk_version >= 21 and not force_append:
+            print("Auto enabled force append mode")
+            force_append = True
         process_list = manifest.get_process_list()
-        authorities = manifest.package_name + '.authorities'
-        print('Add provider %s' % provider_name)
+        authorities = manifest.package_name + ".authorities"
+        print("Add provider %s" % provider_name)
         manifest.add_provider(provider_name, authorities)  # 主进程
         for i, process in enumerate(process_list):
-            sub_provider_name = provider_name + '$InnerClass' + str(i + 1)
-            print('Add provider %s in process %s' %
-                  (sub_provider_name, process))
-            manifest.add_provider(
-                sub_provider_name, authorities + str(i), process)
+            if i < max_child_process:
+                sub_provider_name = provider_name + "$InnerClass" + str(i + 1)
+                print("Add provider %s in process %s" % (sub_provider_name, process))
+                manifest.add_provider(sub_provider_name, authorities + str(i), process)
+            else:
+                print("Add provider ignore process %s" % process)
 
         if activity_list:
             for activity in activity_list:
-                print('Add activity %s' % activity['name'])
+                print("Add activity %s" % activity["name"])
                 manifest.add_activity(
-                    activity['name'], activity['exported'], activity['process'])
+                    activity["name"], activity["exported"], activity["process"]
+                )
 
         # 合并dex文件
-        print('Merge dex %s' % merge_dex_path)
-        classes_dex_path = tempfile.mktemp('.dex')
+        print("Merge dex %s" % merge_dex_path)
+        classes_dex_path = tempfile.mktemp(".dex")
 
         dex_index = 1
         low_memory = False
         while True:
-            dex_file = 'classes%s.dex' % (dex_index if dex_index > 1 else '')
+            dex_file = "classes%s.dex" % (dex_index if dex_index > 1 else "")
             if not apk_file.get_file(dex_file):
                 # 作为最后一个classes.dex
-                with open(merge_dex_path, 'rb') as f:
+                with open(merge_dex_path, "rb") as f:
                     apk_file.add_file(dex_file, f.read())
-                print('Save dex %s to %s' % (merge_dex_path, dex_file))
+                print("Save dex %s to %s" % (merge_dex_path, dex_file))
                 break
 
             if force_append or low_memory:
                 # 低内存下直接跳过已有dex，进行加速
                 dex_index += 1
                 continue
 
             if os.path.exists(classes_dex_path):
                 os.remove(classes_dex_path)
             apk_file.extract_file(dex_file, classes_dex_path)
             try:
-                merge_dex(classes_dex_path, [
-                          classes_dex_path, merge_dex_path], max_heap_size)
+                merge_dex(
+                    classes_dex_path, [classes_dex_path, merge_dex_path], max_heap_size
+                )
             except TooManyMethodsError:
-                print('Merge dex into %s failed due to methods number' % dex_file)
+                print("Merge dex into %s failed due to methods number" % dex_file)
                 dex_index += 1
             except OutOfMemoryError:
-                print('Merge dex into %s failed due to out of memory error' % dex_file)
+                print("Merge dex into %s failed due to out of memory error" % dex_file)
                 low_memory = True
                 dex_index += 1
             else:
-                print('Merge dex into %s success' % dex_file)
-                with open(classes_dex_path, 'rb') as f:
+                print("Merge dex into %s success" % dex_file)
+                with open(classes_dex_path, "rb") as f:
                     apk_file.add_file(dex_file, f.read())
                 break
 
-        if dex_index > 1:
+        if dex_index > 1 and manifest.min_sdk_version < 21:
             # 合并进非主dex只支持5.0以上系统
-            print('WARNING: APK can only be installed in android above 5.0')
+            print("WARNING: APK can only be installed in android above 5.0")
             manifest.min_sdk_version = 21
 
+        # if manifest.target_sdk_version > 27:
+        #     manifest.target_sdk_version = 27
+
         manifest.save()
 
         if res_file_list:
             for src_path, dst_path in res_file_list:
-                with open(src_path, 'rb') as f:
-                    print('Copy file %s => %s' % (src_path, dst_path))
+                with open(src_path, "rb") as f:
+                    print("Copy file %s => %s" % (src_path, dst_path))
                     data = f.read()
                     apk_file.add_file(dst_path, data)
 
-        for it in apk_file.list_dir('META-INF'):
-            if it.lower().endswith('.rsa'):
-                print('Signature file is %s' % it)
-                tmp_rsa_path = tempfile.mktemp('.rsa')
-                apk_file.extract_file('META-INF/%s' % it, tmp_rsa_path)
+        for it in apk_file.list_dir("META-INF"):
+            if it.lower().endswith(".rsa"):
+                print("Signature file is %s" % it)
+                tmp_rsa_path = tempfile.mktemp(".rsa")
+                apk_file.extract_file("META-INF/%s" % it, tmp_rsa_path)
                 orig_signature = get_apk_signature(tmp_rsa_path).strip()
                 os.remove(tmp_rsa_path)
-                logging.info('%s signature is %s' %
-                             (manifest.package_name, orig_signature))
+                logging.info(
+                    "%s signature is %s" % (manifest.package_name, orig_signature)
+                )
                 signature_dict[manifest.package_name] = orig_signature
                 break
         else:
-            raise RuntimeError('Can not find .sf file in META-INF dir')
+            raise RuntimeError("Can not find .sf file in META-INF dir")
 
-        for it in apk_file.list_dir('META-INF'):
-            apk_file.delete_file('META-INF/%s' % it)
+        for it in apk_file.list_dir("META-INF"):
+            apk_file.delete_file("META-INF/%s" % it)
 
     out_apk_list = []
 
     # 写入原始签名信息
-    print('Write original signatures: %s' % json.dumps(signature_dict))
-    temp_dir = tempfile.mkdtemp('-repack')
+    print("Write original signatures: %s" % json.dumps(signature_dict))
+    temp_dir = tempfile.mkdtemp("-repack")
     for i, apk_file in enumerate(apk_file_list):
-        apk_file.add_file('assets/qt4a_package_signatures.txt',
-                          json.dumps(signature_dict))
-        file_name = os.path.split(apk_path_or_list[i])[-1][:-4] + '-repack.apk'
+        apk_file.add_file(
+            "assets/qt4a_package_signatures.txt", json.dumps(signature_dict)
+        )
+        file_name = os.path.split(apk_path_or_list[i])[-1][:-4] + "-repack.apk"
         tmp_apk_path = os.path.join(temp_dir, file_name)
         apk_file.save(tmp_apk_path)
         new_path = resign_apk(tmp_apk_path)
         os.remove(tmp_apk_path)
         out_apk_list.append(new_path)
     if len(out_apk_list) == 1:
         return out_apk_list[0]
     else:
         return out_apk_list
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     pass
```

### Comparing `qt4a-2.3.1/qt4a/apktool/tools/apkhelper.jar` & `qt4a-3.0.0/qt4a/apktool/tools/apkhelper.jar`

 * *Files identical despite different names*

### Comparing `qt4a-2.3.1/qt4a/apktool/tools/asm-debug-all-5.0.3.jar` & `qt4a-3.0.0/qt4a/apktool/tools/asm-debug-all-5.0.3.jar`

 * *Files identical despite different names*

### Comparing `qt4a-2.3.1/qt4a/apktool/tools/d2j-base-cmd-2.1-SNAPSHOT.jar` & `qt4a-3.0.0/qt4a/apktool/tools/d2j-base-cmd-2.1-SNAPSHOT.jar`

 * *Files identical despite different names*

### Comparing `qt4a-2.3.1/qt4a/apktool/tools/dex-ir-2.1-SNAPSHOT.jar` & `qt4a-3.0.0/qt4a/apktool/tools/dex-ir-2.1-SNAPSHOT.jar`

 * *Files identical despite different names*

### Comparing `qt4a-2.3.1/qt4a/apktool/tools/dex-reader-2.1-SNAPSHOT.jar` & `qt4a-3.0.0/qt4a/apktool/tools/dex-reader-2.1-SNAPSHOT.jar`

 * *Files identical despite different names*

### Comparing `qt4a-2.3.1/qt4a/apktool/tools/dex-reader-api-2.1-SNAPSHOT.jar` & `qt4a-3.0.0/qt4a/apktool/tools/dex-reader-api-2.1-SNAPSHOT.jar`

 * *Files identical despite different names*

### Comparing `qt4a-2.3.1/qt4a/apktool/tools/dex-tools-2.1-SNAPSHOT.jar` & `qt4a-3.0.0/qt4a/apktool/tools/dex-tools-2.1-SNAPSHOT.jar`

 * *Files identical despite different names*

### Comparing `qt4a-2.3.1/qt4a/apktool/tools/dex-translator-2.1-SNAPSHOT.jar` & `qt4a-3.0.0/qt4a/apktool/tools/dex-translator-2.1-SNAPSHOT.jar`

 * *Files identical despite different names*

### Comparing `qt4a-2.3.1/qt4a/apktool/tools/dx.jar` & `qt4a-3.0.0/qt4a/apktool/tools/dx.jar`

 * *Files identical despite different names*

### Comparing `qt4a-2.3.1/qt4a/apktool/tools/qt4a.keystore` & `qt4a-3.0.0/qt4a/apktool/tools/qt4a.keystore`

 * *Files identical despite different names*

### Comparing `qt4a-2.3.1/qt4a/browser.py` & `qt4a-3.0.0/qt4a/browser.py`

 * *Files identical despite different names*

### Comparing `qt4a-2.3.1/qt4a/device.py` & `qt4a-3.0.0/qt4a/device.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # -*- coding=utf8 -*-
 #
 # Tencent is pleased to support the open source community by making QTA available.
 # Copyright (C) 2016THL A29 Limited, a Tencent company. All rights reserved.
-# Licensed under the BSD 3-Clause License (the "License"); you may not use this 
+# Licensed under the BSD 3-Clause License (the "License"); you may not use this
 # file except in compliance with the License. You may obtain a copy of the License at
-# 
+#
 # https://opensource.org/licenses/BSD-3-Clause
-# 
-# Unless required by applicable law or agreed to in writing, software distributed 
+#
+# Unless required by applicable law or agreed to in writing, software distributed
 # under the License is distributed on an "AS IS" basis, WITHOUT WARRANTIES OR CONDITIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 #
 
-'''
+"""
 Android 设备模块
-'''
+"""
 
 import six
 import os
 import re
 import socket
 import struct
 import time
@@ -32,597 +32,662 @@
 from testbase import logger as qta_logger
 from testbase.conf import settings
 from testbase.resource import LocalResourceHandler, LocalResourceManagerBackend
 from qt4a.androiddriver.adb import ADB, LocalADBBackend
 from qt4a.androiddriver.util import Singleton, logger, static_property, get_file_md5
 from qt4a.androiddriver.devicedriver import DeviceDriver
 
+
 class AndroidDeviceResourceHandler(LocalResourceHandler):
-    
     def iter_resource(self, res_group=None, condition=None):
         """遍历全部资源（可以按照优先级顺序返回来影响申请资源的优先级）
 
         :param res_group: 资源分组
         :type res_group: str
         :param condition: 资源属性匹配
         :type condition: dict
         :returns: iterator of resource, dict type with key 'id'
         :rtypes: iterator(dict)
         """
         device_list = LocalDeviceProvider.list()
-        
+
         for device in device_list:
-            yield {'id': device}
-            
+            if condition and "id" in condition:
+                device = condition["id"]
+            yield {"id": device}
+
+
 # 注册android本地资源
-LocalResourceManagerBackend.register_resource_type("android", AndroidDeviceResourceHandler())    
+LocalResourceManagerBackend.register_resource_type(
+    "android", AndroidDeviceResourceHandler()
+)
 
-class IDeviceProvider(object):
 
+class IDeviceProvider(object):
     def connect_device(self, dev_prop):
-        '''连接设备
+        """连接设备
 
         :param dev_prop: 设备属性
         :type  dev_prop: dict
 
         :return: Device实例
-        '''
+        """
         pass
 
     def release_device(self, dev_id):
-        '''释放设备
+        """释放设备
 
         :param dev_id: 设备ID
         :type  dev_id: str
-        '''
+        """
         pass
 
+
 class LocalDeviceProvider(IDeviceProvider):
-    '''本地设备提供者
-    '''
+    """本地设备提供者
+    """
 
     @staticmethod
     def list():
-        '''获取本地可用设备列表
-        '''
+        """获取本地可用设备列表
+        """
         device_list = LocalADBBackend.list_device()
         _device_list = []
         for device in device_list:
-            if device.startswith('emulator-'): continue  # 避免出现两个名字不同的同一设备
+            if device.startswith("emulator-"):
+                continue  # 避免出现两个名字不同的同一设备
             _device_list.append(device)
-        available_devices = os.environ.get('QT4A_AVAILABLE_DEVICES', '')
+        available_devices = os.environ.get("QT4A_AVAILABLE_DEVICES", "")
         if _device_list and available_devices:
             intersect_device_list = []
-            available_device_list = available_devices.split(',')
+            available_device_list = available_devices.split(",")
             for available_device in available_device_list:
                 available_device = available_device.strip()
                 if available_device in _device_list:
                     intersect_device_list.append(available_device)
             _device_list = intersect_device_list
 
         import random
+
         random.shuffle(_device_list)  # 可以随机取设备
         return _device_list
 
     def connect_device(self, dev_prop):
-        '''连接设备
+        """连接设备
 
         :param dev_prop: 设备属性
         :type  dev_prop: dict
 
         :return: Device实例
-        '''
-        if not 'id' in dev_prop: return None
-        dev_id = dev_prop['id']
+        """
+        if "id" not in dev_prop or "properties" in dev_prop:
+            # Not local device
+            return None
+        dev_id = dev_prop["id"]
+        logger.info("Connect local device %s" % dev_id)
         if dev_id in LocalDeviceProvider.list():
             return Device(dev_id)
         return None
 
+
 class DeviceProviderManager(Singleton):
-    '''设备提供者管理
-    '''
+    """设备提供者管理
+    """
 
     def __init__(self):
         self._device_providers = [LocalDeviceProvider()]
         for ep in iter_entry_points("qt4a.device_provider"):
             device_provider_class = ep.load()
             self._device_providers.append(device_provider_class())
         self._acquired_devices = {}
 
     def connect_device(self, dev_prop):
-        '''连接设备
+        """连接设备
 
         :param dev_prop: 设备属性
         :type  dev_prop: dict
 
         :return: Device实例
-        '''
+        """
         for provider in self._device_providers:
             device = provider.connect_device(dev_prop)
-            print (device)
-            if device: 
+            if device:
                 self._acquired_devices[device.device_id] = provider
                 return device
         return None
 
     def release_all(self):
-        '''释放所有设备
-        '''
+        """释放所有设备
+        """
         for device_id in self._acquired_devices:
             self._acquired_devices[device_id].release(device_id)
         self._acquired_devices = {}
 
+
 class Device(object):
-    '''Android设备类
-    '''
-    device_list = [] 
+    """Android设备类
+    """
+
+    device_list = []
 
     def __init__(self, id_or_adb_backend=None):
-        '''获取一个Android设备，获取成功后则独占该设备。
+        """获取一个Android设备，获取成功后则独占该设备。
         
         :param device_id: 获取制定设备id的Android设备。如果为空则任意获取一台空闲设备。
-        '''
+        """
         self._device = None
         if isinstance(id_or_adb_backend, str):
             adb_backend = LocalADBBackend.open_device(id_or_adb_backend)
         elif not id_or_adb_backend:
             local_device_list = LocalDeviceProvider.list()
-            if not local_device_list: raise RuntimeError('No local device found')
+            if not local_device_list:
+                raise RuntimeError("No local device found")
             adb_backend = LocalADBBackend.open_device(local_device_list[0])
         else:
             adb_backend = id_or_adb_backend
         self._adb = ADB.open_device(adb_backend)
         self._device_driver = DeviceDriver(self._adb)
         Device.device_list.append(self)
 
     def __del__(self):
-        '释放设备'
+        "释放设备"
         pass
-        
+
     @staticmethod
     def release_all_device():
-        '''释放所有设备
-        '''
-        qta_logger.info('释放设备资源')
+        """释放所有设备
+        """
+        qta_logger.info("释放设备资源")
         Device.device_list = []
         DeviceProviderManager().release_all()
 
     @static_property
     def device_id(self):
-        '''设备ID
-        '''
+        """设备ID
+        """
         return self.adb.device_name
-    
+
     @property
     def device_host(self):
-        '''设备主机
-        '''
+        """设备主机
+        """
         return self.adb.device_host
-        
+
     @static_property
     def cpu_type(self):
-        '''cpu类型
-        '''
+        """cpu类型
+        """
         return self.adb.get_cpu_abi()
 
     @property
     def imei(self):
-        '''手机串号
-        '''
-        if not hasattr(self, '_imei'):
+        """手机串号
+        """
+        if not hasattr(self, "_imei"):
             self._imei = self._device_driver.get_device_imei()
         return self._imei
 
     @static_property
     def model(self):
-        '''设备型号
-        '''
+        """设备型号
+        """
         return self.adb.get_device_model()
 
     @static_property
     def system_version(self):
-        '''系统版本
-        '''
+        """系统版本
+        """
         return self.adb.get_system_version()
 
     @static_property
     def sdk_version(self):
-        '''SDK版本
-        '''
+        """SDK版本
+        """
         return self.adb.get_sdk_version()
 
     @property
     def screen_size(self):
-        '''屏幕大小
-        '''
+        """屏幕大小
+        """
         return self._device_driver.get_screen_size()
-    
+
     @static_property
     def screen_scale(self):
-        '''屏幕缩放比例
-        '''
+        """屏幕缩放比例
+        """
         if self.is_emulator_device():
-            return int(self.adb.get_property('qemu.sf.lcd_density')) / 160.0
+            return int(self.adb.get_property("qemu.sf.lcd_density")) / 160.0
         else:
-            return int(self.adb.get_property('ro.sf.lcd_density')) / 160.0
-    
+            return int(self.adb.get_property("ro.sf.lcd_density")) / 160.0
+
     @property
     def language(self):
-        '''语言
-        '''
+        """语言
+        """
         return self._device_driver.get_language()
 
     @property
     def country(self):
-        '''国家
-        '''
+        """国家
+        """
         return self._device_driver.get_country()
-    
+
     @property
     def current_activity(self):
-        '''当前Activity
-        '''
+        """当前Activity
+        """
         return self.get_current_activity()
-    
+
     @property
     def adb(self):
         return self._adb
-    
+
     @property
     def debuggable(self):
-        '''是否是调试版系统
-        '''
-        return not (self.adb.get_property('ro.secure') == '1' and self.adb.get_property('ro.debuggable') == '0')
+        """是否是调试版系统
+        """
+        return not (
+            self.adb.get_property("ro.secure") == "1"
+            and self.adb.get_property("ro.debuggable") == "0"
+        )
 
     def __str__(self):
-        return '%s(%s %s Android %s)' % (self.device_id, self.model, self.cpu_type, self.system_version)
-    
+        return "%s(%s %s Android %s)" % (
+            self.device_id,
+            self.model,
+            self.cpu_type,
+            self.system_version,
+        )
+
     def get_imei(self):
-        '''获取设备imei号
-        '''
+        """获取设备imei号
+        """
         try:
             return self.adb.get_device_imei()
         except RuntimeError as e:
-            logger.warn('Read device imei by dumpsys failed: %s' % e)
+            logger.warn("Read device imei by dumpsys failed: %s" % e)
             return self._device_driver.get_device_imei()
 
     def is_rooted(self):
-        '''是否root
-        '''
+        """是否root
+        """
         return self.adb.is_rooted()
 
     def is_emulator_device(self):
-        '''是否是模拟器设备
-        '''
-        return self.adb.get_property('ro.kernel.android.qemud').strip() == '1'
-        
+        """是否是模拟器设备
+        """
+        return self.adb.get_property("ro.kernel.android.qemud").strip() == "1"
+
     def run_shell_cmd(self, cmd, *args, **kwargs):
-        '''执行adb shell命令
-        '''
+        """执行adb shell命令
+        """
         return self.adb.run_shell_cmd(cmd, *args, **kwargs)
-    
+
     def run_as(self, package_name, cmd, **kwargs):
-        '''以package_name权限执行命令cmd
+        """以package_name权限执行命令cmd
         
         :param package_name: 包名，必须是已经安装的debug包
         :type  package_name: string
         :param cmd:          命令行
         :type  cmd:          string
-        '''
+        """
         return self.adb.run_as(package_name, cmd, **kwargs)
-    
-    def start_activity(self, activity_name, action='', type='', data_uri='', extra={}, wait=True):
-        '''启动activity
+
+    def start_activity(
+        self, activity_name, action="", type="", data_uri="", extra={}, wait=True
+    ):
+        """启动activity
 
         :param activity_name: Activity名称，如：com.tencent.mobileqq/.activity.SplashActivity
         :type  activity_name: string
         :param action:        Action名称
         :type  action:        string
         :param type:          mime类型
         :type  type:          string
         :param data_uri:      data uri
         :type  data_uri:      string
         :param extra:         额外参数
         :type  extra:         dict
         :param wait:          是否等待启动完成
         :type  wait:          boolean
-        '''
+        """
         use_am = True
 
         for key in extra.keys():
             if isinstance(extra[key], (list, tuple)):
                 use_am = False
                 break
-        if use_am: return self.adb.start_activity(activity_name, action, type, data_uri, extra, wait)
-        
-        params = {'Component': activity_name}
-        if action: params['Action'] = action
-        if type: params['Type'] = type
-        if extra: params['FileUri'] = extra['android.intent.extra.STREAM']
+        if use_am:
+            return self.adb.start_activity(
+                activity_name, action, type, data_uri, extra, wait
+            )
+
+        params = {"Component": activity_name}
+        if action:
+            params["Action"] = action
+        if type:
+            params["Type"] = type
+        if extra:
+            params["FileUri"] = extra["android.intent.extra.STREAM"]
         return self._device_driver.start_activity(params)
 
-    def install_package(self, pkg_path, pkg_name='', overwrite=False):
-        '''安装应用
+    def install_package(self, pkg_path, pkg_name="", overwrite=False):
+        """安装应用
         
         :param pkg_path:  安装包路径
         :type  pkg_path:  string
         :param pkg_name:  应用包名
         :type  pkg_name:  string
         :param overwrite: 是否是覆盖安装
         :type  overwrite: bool
-        '''
+        """
         return self._device_driver.install_package(pkg_path, overwrite)
-    
+
     def uninstall_package(self, pkg_name):
-        '''卸载应用
+        """卸载应用
         
         :param pkg_name: 包名
         :type  pkg_name: string
-        '''
+        """
         return self.adb.uninstall_app(pkg_name)
-        
+
     def kill_process(self, package_name):
-        '''杀死进程
+        """杀死进程
         
         :param package_name: 应用包名
         :type package_name: string
-        '''
+        """
         return self._device_driver.kill_process(package_name)
 
     def push_file(self, src_path, dst_path):
-        '''向手机中拷贝文件
+        """向手机中拷贝文件
         
         :param src_path: PC上的源路径
         :type src_path:  string
         :param dst_path: 手机上的目标路径
         :type dst_path:  string
-        '''
-        
+        """
+
         if not os.path.exists(src_path):
-            raise RuntimeError('File: %s not exist' % src_path)
+            raise RuntimeError("File: %s not exist" % src_path)
         file_size = os.path.getsize(src_path)
         is_zip = False
         if file_size >= 5 * 1024 * 1024:
             is_zip = True
-            zip_file_path = src_path + '.zip'
-            zip_file = zipfile.ZipFile(zip_file_path, 'w', zipfile.ZIP_DEFLATED)
-            if dst_path[-1] == '/':
+            zip_file_path = src_path + ".zip"
+            zip_file = zipfile.ZipFile(zip_file_path, "w", zipfile.ZIP_DEFLATED)
+            if dst_path[-1] == "/":
                 # filename not specified
                 filename = os.path.split(src_path)[-1]
             else:
-                filename = dst_path.split('/')[-1]
+                filename = dst_path.split("/")[-1]
             zip_file.write(src_path, filename)
             zip_file.close()
             src_path = zip_file_path
-            dst_path += '.zip'
+            dst_path += ".zip"
         ret = self.adb.push_file(src_path, dst_path)
         if is_zip:
             os.remove(src_path)
-            if not self._device_driver.unzip_file(dst_path, dst_path[:dst_path.rfind('/')]):
-                logger.warn('unzip file %s failed' % dst_path)
+            if not self._device_driver.unzip_file(
+                dst_path, dst_path[: dst_path.rfind("/")]
+            ):
+                logger.warn("unzip file %s failed" % dst_path)
                 ret = self.adb.push_file(src_path[:-4], dst_path[:-4])
-            elif dst_path.startswith('/data/'):
-                self.adb.chmod(dst_path[:-4], '744')
+            elif dst_path.startswith("/data/"):
+                self.adb.chmod(dst_path[:-4], "744")
             self.delete_file(dst_path)
             dst_path = dst_path[:-4]
         try:
             self.run_shell_cmd('touch "%s"' % dst_path)  # 修改文件修改时间
         except:
-            logger.exception('touch file %s error' % dst_path)
+            logger.exception("touch file %s error" % dst_path)
         return ret
-    
+
     def push_dir(self, src_path, dst_path):
-        '''向手机中拷贝文件夹
+        """向手机中拷贝文件夹
         
         :param src_path: PC上的源目录路径
         :type src_path:  string
         :param dst_path: 手机上的目的目录路径
         :type dst_path:  string
-        '''
+        """
         if not os.path.exists(src_path):
-            raise RuntimeError('Directory %s not exist' % src_path)
+            raise RuntimeError("Directory %s not exist" % src_path)
         for file in os.listdir(src_path):
             file_src_path = os.path.join(src_path, file)
-            file_dst_path = dst_path + '/' + file
+            file_dst_path = dst_path + "/" + file
             self.push_file(file_src_path, file_dst_path)
 
     def pull_file(self, src_path, dst_path):
-        '''将手机中的文件拷贝到PC中
+        """将手机中的文件拷贝到PC中
         
         :param src_path: 手机中的源路径
         :type src_path:  string
         :param dst_path: PC中的目的路径
         :type dst_path:  string
-        '''
+        """
         self.adb.list_dir(src_path)
         try:
             ret = self.adb.pull_file(src_path, dst_path)
-            if 'does not exist' not in ret: return
+            if "does not exist" not in ret:
+                return
         except RuntimeError as e:
-            logger.warn('pull file failed: %r' % e)
-            if src_path.startswith('/data/local/tmp/'): raise e
+            logger.warn("pull file failed: %r" % e)
+            if src_path.startswith("/data/local/tmp/"):
+                raise e
         _, files = self.adb.list_dir(src_path)
         # 需要root权限
-        tmp_path = '/data/local/tmp/%s' % files[0]['name']
+        tmp_path = "/data/local/tmp/%s" % files[0]["name"]
         self.adb.copy_file(src_path, tmp_path)
         self.adb.chmod(tmp_path, 444)
         self.pull_file(tmp_path, dst_path)
         self.adb.delete_file(tmp_path)
 
     def pull_dir(self, src_path, dst_path):
-        '''从手机中拷贝文件夹到PC
+        """从手机中拷贝文件夹到PC
         
         :param src_path: 手机上的源目录路径
         :type src_path:  string
         :param dst_path: PC上的目的目录路径
         :type dst_path:  string
-        '''
+        """
         if not os.path.exists(dst_path):
             os.mkdir(dst_path)
         subdirs, files = self.adb.list_dir(src_path)
         for file in files:
-            self.pull_file(src_path + '/' + file['name'], os.path.join(dst_path, file['name']))
+            self.pull_file(
+                src_path + "/" + file["name"], os.path.join(dst_path, file["name"])
+            )
         for subdir in subdirs:
-            self.pull_dir(src_path + '/' + subdir['name'], os.path.join(dst_path, subdir['name']))
+            self.pull_dir(
+                src_path + "/" + subdir["name"], os.path.join(dst_path, subdir["name"])
+            )
 
     def list_dir(self, dir_path):
-        '''列取目录
-        '''
+        """列取目录
+        """
         return self.adb.list_dir(dir_path)
-    
+
     def is_file_exists(self, file_path):
-        '''判断文件或目录是否存在
+        """判断文件或目录是否存在
 
         :param file_path: 文件或目录在设备中的路径
         :type  file_path: string
-        '''
+        """
         try:
             self.list_dir(file_path)
             return True
         except RuntimeError:
             return False
-        
+
     def delete_folder(self, folder_path):
-        '''删除文件夹
+        """删除文件夹
         
         :param folder_path: 手机中的文件夹路径
         :type folder_path:  string
-        '''
+        """
         return self.adb.delete_folder(folder_path)
 
     def delete_file(self, file_path):
-        '''删除文件
+        """删除文件
 
         :param file_path: 文件在设备中的路径
         :type  file_path: string
-        '''
+        """
         return self.adb.delete_file(file_path)
 
     def mkdir(self, dir_path):
-        '''创建目录
+        """创建目录
 
         :param dir_path: 要创建的目录路径
         :type  dir_path: string
-        '''
+        """
         return self.adb.mkdir(dir_path)
-    
+
     def copy_file(self, src_path, dst_path):
-        '''设备内复制文件
+        """设备内复制文件
         
         :param src_path: 源路径
         :type src_path:  string
         :param dst_path: 目标路径
         :type dst_path:  string
-        '''
+        """
         if not self.is_file_exists(src_path):
-            raise RuntimeError('File %s not exist' % src_path)
+            raise RuntimeError("File %s not exist" % src_path)
         self.adb.copy_file(src_path, dst_path)
-        
+
     def get_external_sdcard_path(self):
-        '''获取外置SD卡路径
-        '''
+        """获取外置SD卡路径
+        """
         return self._device_driver.get_external_sdcard_path()
 
-    def refresh_media_store(self, file_path=''):
-        '''刷新图库，显示新拷贝到手机的图片
+    def refresh_media_store(self, file_path=""):
+        """刷新图库，显示新拷贝到手机的图片
 
         :param file_path: 要刷新的图片路径，不指定则刷新整个sdcard
         :type  file_path: string
-        '''
+        """
         return self._device_driver.refresh_media_store(file_path)
 
     def get_current_activity(self):
-        '''获取当前Activtiy
-        '''
+        """获取当前Activtiy
+        """
         return self._device_driver.get_current_activity()
 
     def take_screen_shot(self, save_path):
-        '''截屏
+        """截屏
         
         :param save_path: 截屏图片存放在PC上的路径
         :type save_path: string
-        '''
+        """
         return self._device_driver.take_screen_shot(save_path)
-    
+
     def record_screen(self, save_path, record_time, frame_rate=10, quality=20):
-        '''录屏
+        """录屏
         
         :param save_path:   保存路径，如果为已存在的目录路径，则会将每一帧图片保存到该目录下
         :type  save_path:   string
         :param record_time: 录制时间，单位：秒
         :type  record-time: int/float
         :param frame_rate:  帧率，1-30
         :type  frame_rate:  int
         :param quality:     压缩质量，10-100
         :type  quality:     int
-        '''
+        """
         import shutil
         from qt4a.androiddriver.device_driver import qt4a_path
+
         to_video = True
-        if os.path.exists(save_path) and os.path.isdir(save_path): to_video = False
-        
+        if os.path.exists(save_path) and os.path.isdir(save_path):
+            to_video = False
+
         if frame_rate < 1 or frame_rate > 30:
-            raise ValueError('frame rate must between 1 and 30')
+            raise ValueError("frame rate must between 1 and 30")
         if quality < 10 or quality > 100:
-            raise ValueError('quality must between 10 and 100')
-        remote_tmp_path = '%s/screen.record' % qt4a_path
-        self.run_shell_cmd('%s/screenshot record -p %s -t %d -f %d -q %d' % (qt4a_path, remote_tmp_path, int(record_time * 1000), int(frame_rate), int(quality)))
+            raise ValueError("quality must between 10 and 100")
+        remote_tmp_path = "%s/screen.record" % qt4a_path
+        self.run_shell_cmd(
+            "%s/screenshot record -p %s -t %d -f %d -q %d"
+            % (
+                qt4a_path,
+                remote_tmp_path,
+                int(record_time * 1000),
+                int(frame_rate),
+                int(quality),
+            )
+        )
         local_tmp_path = tempfile.mktemp()
         self.pull_file(remote_tmp_path, local_tmp_path)
         save_dir = save_path
-        if to_video: save_dir = tempfile.mkdtemp('.screenshot')
+        if to_video:
+            save_dir = tempfile.mkdtemp(".screenshot")
         frame_list = Device.extract_record_frame(local_tmp_path, save_dir)
         os.remove(local_tmp_path)
         if to_video:
             Device.screen_frame_to_video(frame_list, frame_rate, save_path)
             shutil.rmtree(save_dir)
         result = []
         for it in os.listdir(save_dir):
             result.append(os.path.join(save_dir, it))
         return result
-    
+
     @staticmethod
     def screen_frame_to_video(frame_list, frame_rate, save_path):
-        '''将录屏帧序列转换为视频文件
-        '''
+        """将录屏帧序列转换为视频文件
+        """
         try:
             import cv2
         except ImportError:
             return None
-        
+
         _, width, height = cv2.imread(frame_list[0]).shape[::-1]
-        format = 'MJPG'
-        if save_path.lower().endswith('.flv'): format = 'FLV1'
-        elif save_path.lower().endswith('.mp4'): format = 'DIVX'
-        videoWriter = cv2.VideoWriter(save_path, cv2.VideoWriter_fourcc(*format), frame_rate, (width, height))
+        format = "MJPG"
+        if save_path.lower().endswith(".flv"):
+            format = "FLV1"
+        elif save_path.lower().endswith(".mp4"):
+            format = "DIVX"
+        videoWriter = cv2.VideoWriter(
+            save_path, cv2.VideoWriter_fourcc(*format), frame_rate, (width, height)
+        )
         for it in frame_list:
-            img = cv2.imread(it) 
+            img = cv2.imread(it)
             videoWriter.write(img)
         return save_path
-            
+
     @staticmethod
     def extract_record_frame(file_path, save_dir):
-        '''提取录屏文件中的帧
-        '''
+        """提取录屏文件中的帧
+        """
         frame_list = []
-        with open(file_path, 'rb') as fp:
+        with open(file_path, "rb") as fp:
             while True:
                 data = fp.read(4)
-                if not data: break
-                timestamp = struct.unpack('I', data)[0]
-                data_len = struct.unpack('I', fp.read(4))[0]
+                if not data:
+                    break
+                timestamp = struct.unpack("I", data)[0]
+                data_len = struct.unpack("I", fp.read(4))[0]
                 data = fp.read(data_len)
-                save_path = os.path.join(save_dir, '%.8d.jpg' % timestamp)
-                with open(save_path, 'wb') as f:
+                save_path = os.path.join(save_dir, "%.8d.jpg" % timestamp)
+                with open(save_path, "wb") as f:
                     f.write(data)
                 frame_list.append(save_path)
         return frame_list
-    
-    def drag(self, x1, y1, x2, y2, count=5, wait_time=40, send_down_event=True, send_up_event=True):
-        '''滑动
+
+    def drag(
+        self,
+        x1,
+        y1,
+        x2,
+        y2,
+        count=5,
+        wait_time=40,
+        send_down_event=True,
+        send_up_event=True,
+    ):
+        """滑动
         
         :param x1: 起始x坐标
         :type x1:  int
         :param y1: 起始y坐标
         :type y1:  int
         :param x2: 终止x坐标
         :type x2:  int
@@ -632,711 +697,828 @@
         :type count:  int
         :param wait_time: 每步间等待的时长
         :type wait_time:  int，单位：ms
         :param send_down_event: 是否发送DOWN事件
         :type  send_down_event: bool
         :param send_up_event: 是否发送UP事件
         :type  send_up_event: bool
-        '''
-        return self._device_driver.drag(x1, y1, x2, y2, count, wait_time, send_down_event, send_up_event)
+        """
+        return self._device_driver.drag(
+            x1, y1, x2, y2, count, wait_time, send_down_event, send_up_event
+        )
 
     def click(self, x, y):
-        '''单击屏幕坐标
+        """单击屏幕坐标
 
         :param x: 横坐标
         :type  x: int/float
         :param y: 纵坐标
         :type  y: int/float
-        '''
+        """
         return self._device_driver.drag(x, y, x, y)
 
     def long_click(self, x, y, duration=1):
-        '''长按屏幕坐标
+        """长按屏幕坐标
 
         :param x: 横坐标
         :type  x: int/float
         :param y: 纵坐标
         :type  y: int/float
         :param duration: 按住时长，单位为秒
         :type duration:  int/float
-        '''
+        """
         self._device_driver.drag(x, y, x, y, send_up_event=False)
         time.sleep(duration)
         self._device_driver.drag(x, y, x, y, send_down_event=False)
 
     def reboot(self, wait_cpu_low=True, usage=20, duration=10, timeout=120):
-        '''重启手机
+        """重启手机
         
         :param wait_cpu_low:   是否等待CPU使用率降低
         :type wait_cpu_low:    bool
         :param usage:          cpu使用率阈值
         :type  usage:          int
         :param duration:       持续时间(秒)
         :type  duration:       int
         :param timeout:        超时时间，超市时间到后，无论当前CPU使用率是多少，都会返回
         :type  timeout:        int
-        '''
-        return self._device_driver.reboot(wait_cpu_low, usage=usage, duration=duration, timeout=timeout)
+        """
+        return self._device_driver.reboot(
+            wait_cpu_low, usage=usage, duration=duration, timeout=timeout
+        )
 
-    def connect_wifi(self, wifi_name, wifi_pass=''):
-        '''连接指定的Wifi
+    def connect_wifi(self, wifi_name, wifi_pass=""):
+        """连接指定的Wifi
         
         :param wifi_name: WiFi名称
         :type wifi_name:  string
-        '''
+        """
         for _ in range(3):
-            if self._device_driver.connect_wifi(wifi_name, wifi_pass): return True
+            if self._device_driver.connect_wifi(wifi_name, wifi_pass):
+                return True
             self.disable_wifi()  # 有些手机需要禁用一下wifi才能正常连接
             time.sleep(10)
         return False
-    
+
     def enable_wifi(self):
-        '''启用Wifi
-        '''
-        ssid = ''
-        pwd = ''
+        """启用Wifi
+        """
+        ssid = ""
+        pwd = ""
 
-        if hasattr(settings, 'QT4A_WIFI_SSID'):
+        if hasattr(settings, "QT4A_WIFI_SSID"):
             ssid = settings.QT4A_WIFI_SSID
-        if hasattr(settings, 'QT4A_WIFI_PASSWORD'):
+        if hasattr(settings, "QT4A_WIFI_PASSWORD"):
             pwd = settings.QT4A_WIFI_PASSWORD
 
-        if ssid: return self.connect_wifi(ssid, pwd)
+        if ssid:
+            return self.connect_wifi(ssid, pwd)
 
         return False
 
     def disable_wifi(self):
-        '''禁用Wifi
-        '''
+        """禁用Wifi
+        """
         return self._device_driver.disable_wifi()
-    
+
     def switch_to_data_connection(self):
-        '''关闭WIFI,启用数据连接
-        '''
+        """关闭WIFI,启用数据连接
+        """
         return self.disable_wifi() and self._device_driver.enable_data_connection()
 
     def disable_data_connection(self):
-        '''禁用数据连接
-        '''
+        """禁用数据连接
+        """
         sim_state = self.get_sim_card_state()
-        if 'SIM_STATE_ABSENT' in sim_state or 'SIM_STATE_UNKNOWN' in sim_state: return True
+        if "SIM_STATE_ABSENT" in sim_state or "SIM_STATE_UNKNOWN" in sim_state:
+            return True
         return self._device_driver.disable_data_connection()
 
     def disable_network(self):
-        '''禁用所有网络
-        '''
+        """禁用所有网络
+        """
         return self.disable_wifi() and self.disable_data_connection()
 
     def enable_network(self):
-        '''启用任一网络，优先使用Wifi
-        '''
+        """启用任一网络，优先使用Wifi
+        """
         return self.enable_wifi() or self.enable_data_connection()
 
     def read_logcat(self, tag, process_name_pattern, pattern, num=1):
-        '''查找最近满足条件的一条log
+        """查找最近满足条件的一条log
         
         :param tag: 期望的Tag
         :type tag:  string
         :param process_name_pattern: 期望的进程名，传入正则表达式
         :type process_name_pattern:  string
         :param pattern:  期望匹配的格式
         :type pattern:   Pattern
         :param num:  返回满足条件的日志条数
         :type num:   int
-        '''
+        """
         from qt4a.androiddriver.util import logger
-        pat = re.compile(r'^\[(.+)\(\d+\)\]\s+\[.+\]\s+\w/(.+)\(\s*\d+\):\s+(.+)$')
+
+        pat = re.compile(r"^\[(.+)\(\d+\)\]\s+\[.+\]\s+\w/(.+)\(\s*\d+\):\s+(.+)$")
         log_pat = re.compile(pattern)
         log_list = self.adb.get_log(False)
         log_list = [i.decode("utf-8") for i in log_list]
         result_list = []
         k = 0
         for i in range(len(log_list) - 1, -1, -1):
             ret = pat.match(log_list[i])
-            if not ret: 
-                logger.info('read_logcat:%s not match ^\[(.+)\(\d+\)\]\s+\[.+\]\s+\w/(.+)\(\s*\d+\):\s+(.+)$' % log_list[i])
+            if not ret:
+                logger.info(
+                    "read_logcat:%s not match ^\[(.+)\(\d+\)\]\s+\[.+\]\s+\w/(.+)\(\s*\d+\):\s+(.+)$"
+                    % log_list[i]
+                )
+                continue
+            if not process_name_pattern:
                 continue
-            if not process_name_pattern: continue
             process_pat = re.compile(process_name_pattern)
-            if not process_pat.match(ret.group(1)): continue
-            if ret.group(2) != tag: continue
+            if not process_pat.match(ret.group(1)):
+                continue
+            if ret.group(2) != tag:
+                continue
             if log_pat.search(ret.group(3)):
                 if num == 1:
                     return ret.group(3)
                 elif num == 0 or k < num:
                     k += 1
                     result_list.append(ret.group(3))
                 else:
                     break
         return result_list
 
     def get_clipboard_text(self):
-        '''获取剪切板内容
-        '''
+        """获取剪切板内容
+        """
         return self._device_driver.get_clipboard_text()
-    
+
     def set_clipboard_text(self, text):
-        '''设置剪贴板内容
-        '''
+        """设置剪贴板内容
+        """
         return self._device_driver.set_clipboard_text(text)
-    
+
     def wake_screen(self, wake=True):
-        '''唤醒屏幕
-        '''
+        """唤醒屏幕
+        """
         return self._device_driver.wake_screen(wake)
 
     def unlock_keyguard(self):
-        '''解锁屏幕
-        '''
+        """解锁屏幕
+        """
         return self._device_driver.unlock_keyguard()
-    
+
     def lock_keyguard(self):
-        '''锁屏
-        '''
+        """锁屏
+        """
         return self._device_driver.lock_keyguard()
-    
+
     def send_key(self, key):
-        '''发送按键
+        """发送按键
         
         :param key: 按键
         :type key:  string
-        '''
+        """
         return self._device_driver.send_key(key)
-    
+
     def send_text(self, text):
-        '''通过输入法方式发送文本
+        """通过输入法方式发送文本
         
         :param text: 要发送的文本
         :type  text: string
-        '''
+        """
         max_send_size = 960
         if isinstance(text, bytes):
-            text = text.decode('utf8')
-        text_en = ''
+            text = text.decode("utf8")
+        text_en = ""
         i = 0
         while i < len(text):
             c = text[i]
-            if c >= u'\ud800' and c <= u'\udbff':
+            if c >= u"\ud800" and c <= u"\udbff":
                 d = text[i + 1]
-                if d >= u'\udc00' and d <= u'\udfff':
+                if d >= u"\udc00" and d <= u"\udfff":
                     # 四字节unicode编码
-                    text_en += r'\u%.4x\u%.4x' % (ord(c), ord(d))
+                    text_en += r"\u%.4x\u%.4x" % (ord(c), ord(d))
                     i += 2
                     continue
             text_en += c
             i += 1
-        
-        text_en = text_en.encode('raw_unicode_escape')
+
+        text_en = text_en.encode("raw_unicode_escape")
         total_len = len(text_en)
-        if total_len > max_send_size: raise RuntimeError('Text is too long %d' % total_len)
-        extra = {'text': text_en}
-        if len(text_en) == 1: extra['toClear'] = 'false'
-        self.adb.send_broadcast('com.test.androidspy.input', extra)
-        
+        if total_len > max_send_size:
+            raise RuntimeError("Text is too long %d" % total_len)
+        extra = {"text": text_en}
+        if len(text_en) == 1:
+            extra["toClear"] = "false"
+        self.adb.send_broadcast("com.test.androidspy.input", extra)
+
     def clear_data(self, package_name):
-        '''清理应用数据
+        """清理应用数据
         
         :param package_name: 包名
         :type package_name:  string
-        '''
-        if not self.adb.get_package_path(package_name): return True
-        cmdline = 'pm clear %s' % package_name
+        """
+        if not self.adb.get_package_path(package_name):
+            return True
+        cmdline = "pm clear %s" % package_name
         if self.adb.is_rooted():
-            return 'Success' in self.run_shell_cmd(cmdline, True)
+            return "Success" in self.run_shell_cmd(cmdline, True)
         else:
             result = self.run_shell_cmd(cmdline)
-            if 'Success' in result:
+            if "Success" in result:
                 return True
-            logger.warn('clear %s data failed: %s' % (package_name, result))
-            return 'Success' in self.run_as(package_name, cmdline)
+            logger.warn("clear %s data failed: %s" % (package_name, result))
+            return "Success" in self.run_as(package_name, cmdline)
 
-    def get_string_resource(self, pkg_name, string_id, lang=''):
-        '''获取字符串资源
-        '''
+    def get_string_resource(self, pkg_name, string_id, lang=""):
+        """获取字符串资源
+        """
         result = self._device_driver.get_string_resource(pkg_name, string_id, lang)
-        if result == ("Can't find string %s" % string_id) or 'Can\'t find class' in result:
-            if pkg_name == 'android': raise RuntimeError(result)
-            return self.get_string_resource('android', string_id, lang)
+        if (
+            result == ("Can't find string %s" % string_id)
+            or "Can't find class" in result
+        ):
+            if pkg_name == "android":
+                raise RuntimeError(result)
+            return self.get_string_resource("android", string_id, lang)
         else:
             return result
-        
+
     def get_string_resource_id(self, pkg_name, text):
-        '''获取字符串资源ID
-        '''
+        """获取字符串资源ID
+        """
         return self._device_driver.get_string_resource_id(pkg_name, text)
 
     def set_default_language(self, lang):
-        '''设置默认语言
-        '''
+        """设置默认语言
+        """
         return self._device_driver.set_default_language(lang)
 
     def is_app_installed(self, app_name):
-        '''应用是否安装
-        '''
+        """应用是否安装
+        """
         package_path = self.adb.get_package_path(app_name)
-        return package_path != ''
+        return package_path != ""
 
-    def get_static_field_value(self, pkg_name, cls_name, field_name, field_type=''):
-        '''获取类中静态变量的值
+    def get_static_field_value(self, pkg_name, cls_name, field_name, field_type=""):
+        """获取类中静态变量的值
         
         :param pkg_name:   包名
         :type pkg_name:    string
         :param cls_name:   类名
         :type cls_name:    string
         :param field_name: 字段名
         :type field_name:  string 
-        '''
-        return self._device_driver.get_static_field_value(pkg_name, cls_name, field_name, field_type)
+        """
+        return self._device_driver.get_static_field_value(
+            pkg_name, cls_name, field_name, field_type
+        )
 
     def set_default_app(self, action, type, new_app):
-        '''设置默认应用
+        """设置默认应用
         
         :param action:  应用针对的类型，如：android.media.action.IMAGE_CAPTURE
         :type  action:  String
         :param new_app: 新的应用包名
         :type  new_app: String
-        '''
+        """
         return self._device_driver.set_default_app(action, type, new_app)
-    
+
     def set_camera_photo(self, pic_path):
-        '''设置相机图片，调用该接口后，调用相机接口会返回指定图片
+        """设置相机图片，调用该接口后，调用相机接口会返回指定图片
         
         :param pic_path: 图片在PC中的路径
         :type pic_path:  String
-        '''
+        """
         if not os.path.exists(pic_path):
-            raise RuntimeError('图片：%s 不存在' % pic_path)
-        dst_path = '/sdcard/dcim/camera%s' % (os.path.splitext(pic_path)[1])
+            raise RuntimeError("图片：%s 不存在" % pic_path)
+        dst_path = "/sdcard/dcim/camera%s" % (os.path.splitext(pic_path)[1])
         self.push_file(pic_path, dst_path)
-        self.adb.set_property('debug.mockcamera.image_path', dst_path)
-        self.set_default_app('android.media.action.IMAGE_CAPTURE', '', 'com.test.androidspy')
-    
+        self.adb.set_property("debug.mockcamera.image_path", dst_path)
+        self.set_default_app(
+            "android.media.action.IMAGE_CAPTURE", "", "com.test.androidspy"
+        )
+
     def clear_camera_default_app(self):
-        '''清除默认相机应用
-        '''
+        """清除默认相机应用
+        """
         from qt4a.androiddriver.util import logger
+
         if self.is_rooted():
-            return self._device_driver.clear_default_app('android.media.action.IMAGE_CAPTURE')
+            return self._device_driver.clear_default_app(
+                "android.media.action.IMAGE_CAPTURE"
+            )
         else:
-            logger.warn('clear_camera_default_app need root')
-           
+            logger.warn("clear_camera_default_app need root")
+
     def has_gps(self):
-        '''是否有GPS
-        '''
+        """是否有GPS
+        """
         return self._device_driver.has_gps()
-    
+
     def has_camera(self):
-        '''是否有摄像头
-        '''
+        """是否有摄像头
+        """
         return self._device_driver.get_camera_number() > 0
 
     def get_sim_card_state(self):
-        '''获取sim卡状态
-        '''
-        sim_state = self.adb.get_property('gsm.sim.state').strip()
-        if sim_state == 'READY': return 'SIM_STATE_READY'
-        if 'ABSENT' in sim_state or 'NOT_READY' in sim_state:
-            return 'SIM_STATE_ABSENT'
-        logger.info('sim state: %s' % sim_state)
-        return 'SIM_STATE_UNKNOWN'
-    
+        """获取sim卡状态
+        """
+        sim_state = self.adb.get_property("gsm.sim.state").strip()
+        if sim_state == "READY":
+            return "SIM_STATE_READY"
+        if "ABSENT" in sim_state or "NOT_READY" in sim_state:
+            return "SIM_STATE_ABSENT"
+        logger.info("sim state: %s" % sim_state)
+        return "SIM_STATE_UNKNOWN"
+
     def has_sim_card(self):
-        '''是否有sim卡
-        '''
+        """是否有sim卡
+        """
         sim_state = self.get_sim_card_state()
-        return sim_state != 'SIM_STATE_ABSENT' and sim_state != 'SIM_STATE_UNKNOWN'  # 虚拟机返回的状态是SIM_STATE_UNKNOWN
-    
+        return (
+            sim_state != "SIM_STATE_ABSENT" and sim_state != "SIM_STATE_UNKNOWN"
+        )  # 虚拟机返回的状态是SIM_STATE_UNKNOWN
+
     def is_debug_package(self, package_name):
-        '''是否是debug包
-        '''
+        """是否是debug包
+        """
         return self._device_driver.is_debug_package(package_name)
-    
+
     def _get_view_id(self, package_name, str_id):
-        '''从控件字符串ID获取整型ID
+        """从控件字符串ID获取整型ID
         
         :param package_name: 应用包名
         :type package_name: string
         :param str_id: 字符串ID
         :type str_id:  string
-        '''
-        if not hasattr(self, '_view_id_dict'):
+        """
+        if not hasattr(self, "_view_id_dict"):
             self._view_id_dict = {}  # 该操作较为耗时，必须要缓存
         if not package_name in self._view_id_dict:
             self._view_id_dict[package_name] = {}
         if str_id in self._view_id_dict[package_name]:
             return self._view_id_dict[package_name][str_id]
         view_id = self._device_driver.get_view_id(package_name, str_id)
         self._view_id_dict[package_name][str_id] = view_id
         return view_id
-    
+
     def _get_resource_origin_name(self, package_name, res_type, confuse_name):
-        '''根据获取资源混淆后的名称获取原始名称
+        """根据获取资源混淆后的名称获取原始名称
         
         :param package_name: 应用包名
         :type package_name:  string
         :param res_type:     资源类型
         :type res_type:      string
         :param confuse_name: 混淆后的名称
         :type confuse_name:  string
-        '''
-        if confuse_name == '': return ''  # 处理空字符串情况
-        if len(confuse_name) > 4: return confuse_name  # 必然没有混淆
-        if not hasattr(self, '_resource_name'):
+        """
+        if confuse_name == "":
+            return ""  # 处理空字符串情况
+        if len(confuse_name) > 4:
+            return confuse_name  # 必然没有混淆
+        if not hasattr(self, "_resource_name"):
             self._resource_name = {}  # 进行缓存
         if not package_name in self._resource_name:
             self._resource_name[package_name] = {}
         if not confuse_name in self._resource_name[package_name]:
-            self._resource_name[package_name][confuse_name] = self._device_driver.get_resource_origin_name(package_name, res_type, confuse_name)
+            self._resource_name[package_name][
+                confuse_name
+            ] = self._device_driver.get_resource_origin_name(
+                package_name, res_type, confuse_name
+            )
         return self._resource_name[package_name][confuse_name]
-    
+
     def send_text_to_app(self, activity, text):
-        '''向app分享文本
-        '''
-        return self.start_activity(activity, action='android.intent.action.SEND', type='text/plain', extra={'android.intent.extra.TEXT': text})
-    
+        """向app分享文本
+        """
+        return self.start_activity(
+            activity,
+            action="android.intent.action.SEND",
+            type="text/plain",
+            extra={"android.intent.extra.TEXT": text},
+        )
+
     def send_image_to_app(self, activity, image_path):
-        '''向app分享图片
-        '''
+        """向app分享图片
+        """
+
         def _copy_image(src_path):
             from qt4a.androiddriver.util import get_file_md5
-            if six.PY2 and not isinstance(src_path, unicode): src_path = src_path.decode('utf8')
+
+            if six.PY2 and not isinstance(src_path, unicode):
+                src_path = src_path.decode("utf8")
             file_ext = os.path.splitext(src_path)[-1]
-            dst_path = '/sdcard/dcim/%s%s' % (get_file_md5(src_path), file_ext)
+            dst_path = "/sdcard/dcim/%s%s" % (get_file_md5(src_path), file_ext)
             self.push_file(src_path, dst_path)
             return dst_path
-        
-        action = 'android.intent.action.SEND'
+
+        action = "android.intent.action.SEND"
         if isinstance(image_path, (list, tuple)):
             image_path_new = [None for _ in range(len(image_path))]
             for i in range(len(image_path)):
-                image_path_new[i] = 'file://' + _copy_image(image_path[i])
+                image_path_new[i] = "file://" + _copy_image(image_path[i])
             image_path = image_path_new
-            action = 'android.intent.action.SEND_MULTIPLE'
+            action = "android.intent.action.SEND_MULTIPLE"
         else:
-            image_path = 'file://' + _copy_image(image_path)
-        return self.start_activity(activity, action=action, type='image/*', extra={'android.intent.extra.STREAM': image_path})
-    
+            image_path = "file://" + _copy_image(image_path)
+        return self.start_activity(
+            activity,
+            action=action,
+            type="image/*",
+            extra={"android.intent.extra.STREAM": image_path},
+        )
+
     def send_file_to_app(self, activity, file_path):
-        '''向app分享文件
-        '''
+        """向app分享文件
+        """
+
         def _copy_file(src_path):
-            if six.PY2 and not isinstance(src_path, unicode): src_path = src_path.decode('utf8')
+            if six.PY2 and not isinstance(src_path, unicode):
+                src_path = src_path.decode("utf8")
             file_name = os.path.split(src_path)[-1]
-            dst_path = '/data/local/tmp/%s' % (file_name)
+            dst_path = "/data/local/tmp/%s" % (file_name)
             self.push_file(src_path, dst_path)
             return dst_path
-        file_path = 'file://' + _copy_file(file_path)
-        return self.start_activity(activity, action='android.intent.action.SEND', type='application/octet-stream', extra={'android.intent.extra.STREAM': file_path})
-    
+
+        file_path = "file://" + _copy_file(file_path)
+        return self.start_activity(
+            activity,
+            action="android.intent.action.SEND",
+            type="application/octet-stream",
+            extra={"android.intent.extra.STREAM": file_path},
+        )
+
     def check_netstat(self):
-        '''检查网络状态
-        '''
+        """检查网络状态
+        """
         try:
-            return 'bytes from' in self.run_shell_cmd('ping -c 1 www.qq.com', self.is_rooted())
+            return "bytes from" in self.run_shell_cmd(
+                "ping -c 1 www.qq.com", self.is_rooted()
+            )
         except TimeoutError:
             return False
-    
+
     def play_sound(self, file_path, volume=50):
-        '''播放语音
+        """播放语音
         
         :param file_path: 音频文件路径
         :type  file_path: string
-        '''
+        """
         from qt4a.androiddriver.util import get_file_md5
+
         self.set_volume(volume)  # 先设置音量
         file_ext = os.path.splitext(file_path)[-1]
-        dst_path = '/data/local/tmp/%s%s' % (get_file_md5(file_path), file_ext)
+        dst_path = "/data/local/tmp/%s%s" % (get_file_md5(file_path), file_ext)
         self.push_file(file_path, dst_path)
         return self._device_driver.play_sound(dst_path)
 
     def modify_hosts(self, new_hosts=[]):
-        '''修改hosts
+        """修改hosts
         
         :param new_hosts: 要修改的host列表,如果为空,表示恢复为默认hosts
         :type new_hosts: list
-        '''
-        hosts_path = '/system/etc/hosts'
-        bak_hosts_path = hosts_path + '.bak'
+        """
+        hosts_path = "/system/etc/hosts"
+        bak_hosts_path = hosts_path + ".bak"
         self.adb._set_system_writable()  # 需要system目录可写
         backup = 'echo "127.0.0.1        localhost" > %s' % (hosts_path)
         if new_hosts:
             if not self.is_file_exists(bak_hosts_path):
                 # 先生成备份文件
                 self.copy_file(hosts_path, bak_hosts_path)
-            
+
             result = self.run_shell_cmd(backup, True)  # 保证当前的hosts文件是干净的
-            if 'Permission denied' in result:
-                self.run_shell_cmd('chmod 666 %s' % hosts_path, True)
+            if "Permission denied" in result:
+                self.run_shell_cmd("chmod 666 %s" % hosts_path, True)
                 self.run_shell_cmd(backup, True)
 
             for ip, host in new_hosts:
-                self.run_shell_cmd('echo "%s        %s" >> %s' % (ip, host, hosts_path), True)
+                self.run_shell_cmd(
+                    'echo "%s        %s" >> %s' % (ip, host, hosts_path), True
+                )
 
             for ip, host in new_hosts:
                 real_ip = self.resolve_domain(host)
                 if real_ip != ip:
-                    raise RuntimeError('设置hosts[%s %s]失败，当前解析值为：%s' % (ip, host, real_ip))
+                    raise RuntimeError(
+                        "设置hosts[%s %s]失败，当前解析值为：%s" % (ip, host, real_ip)
+                    )
         else:
             # 恢复默认的hosts
             if self.is_file_exists(bak_hosts_path):
                 self.copy_file(bak_hosts_path, hosts_path)
             else:
                 self.run_shell_cmd(backup, True)
 
     def set_volume(self, volume):
-        '''设置音量
-        '''
+        """设置音量
+        """
         return self._device_driver.set_volume(volume)
-        
+
     def get_phone_contacts(self):
-        '''获取手机联系人列表
-        '''
+        """获取手机联系人列表
+        """
         return self._device_driver.get_phone_contacts()
-        
+
     def add_phone_contacts(self, name, phone):
-        '''添加手机联系人
-        '''
+        """添加手机联系人
+        """
         return self._device_driver.add_phone_contacts(name, phone)
-    
+
     def del_phone_contacts(self, name):
-        '''删除手机联系人
-        '''
+        """删除手机联系人
+        """
         return self._device_driver.del_phone_contacts(name)
-    
+
     def set_app_permission(self, package_name, perm_name, is_allowed=True):
-        '''设置应用权限
+        """设置应用权限
         
         :param package_name: 应用包名
         :type package_name:  string
         :param perm_name:    权限名称
         :type perm_name:     string
         :param is_allowed:   是否允许
         :type is_allowed:    bool
-        '''
-        return self._device_driver.set_app_permission(package_name, perm_name, is_allowed)
-    
+        """
+        return self._device_driver.set_app_permission(
+            package_name, perm_name, is_allowed
+        )
+
     def set_screen_off_time(self, timeout=600):
-        '''设置灭屏时间
+        """设置灭屏时间
         
         :param timeout: 超时时间
         :type timeout:  int，单位为秒
-        '''
-        if timeout <= 0: timeout = 2147483647
-        else: timeout = timeout * 1000
-        return self._device_driver.modify_system_setting('system', 'screen_off_timeout', timeout)
-    
+        """
+        if timeout <= 0:
+            timeout = 2147483647
+        else:
+            timeout = timeout * 1000
+        return self._device_driver.modify_system_setting(
+            "system", "screen_off_timeout", timeout
+        )
+
     def set_auto_rotate_screen(self, rotate=False):
-        '''设置是否旋转屏幕
+        """设置是否旋转屏幕
         
         :param rotate: 是否旋转
         :type rotate:  boolean
-        '''
-        return self._device_driver.modify_system_setting('system', 'accelerometer_rotation', 1 if rotate else 0)
-    
+        """
+        return self._device_driver.modify_system_setting(
+            "system", "accelerometer_rotation", 1 if rotate else 0
+        )
+
     def set_time_12_24(self, is_24=True):
-        '''设置12/24小时格式
+        """设置12/24小时格式
         
         :param is_24: 是否是24小时
         :type is_24:  boolean
-        '''
-        return self._device_driver.modify_system_setting('system', 'time_12_24', 24 if is_24 else 12)
-    
+        """
+        return self._device_driver.modify_system_setting(
+            "system", "time_12_24", 24 if is_24 else 12
+        )
+
     def set_allow_unknown_app(self, allow=True):
-        '''设置是否允许安装未知来源的应用
+        """设置是否允许安装未知来源的应用
         
         :param allow: 是否允许
         :type allow:  boolean
-        '''
-        return self._device_driver.modify_system_setting('secure', 'install_non_market_apps', 1 if allow else 0)
-    
+        """
+        return self._device_driver.modify_system_setting(
+            "secure", "install_non_market_apps", 1 if allow else 0
+        )
+
     def set_default_input_method(self, input_method):
-        '''设置默认输入法
+        """设置默认输入法
         
         :param input_method: 要设置的输入法服务名（package_name/service_name）
         :type  input_method: string
-        '''
-        self._device_driver.modify_system_setting('secure', 'enabled_input_methods', input_method)
-        self._device_driver.modify_system_setting('secure', 'default_input_method', input_method)
-    
+        """
+        self._device_driver.modify_system_setting(
+            "secure", "enabled_input_methods", input_method
+        )
+        self._device_driver.modify_system_setting(
+            "secure", "default_input_method", input_method
+        )
+
     def connect_vpn(self, vpn_type, server, username, password):
-        '''连接VPN
+        """连接VPN
         
         :param vpn_type:  VPN类型
         :type vpn_type:   string
         :param server:    服务器地址
         :type server:     string
         :param username:  用户名
         :type username:   string
         :param password:  密码
         :type password:   string
-        '''
-        if vpn_type == 'PPTP':
+        """
+        if vpn_type == "PPTP":
             vpn_type = 0
-        elif vpn_type == 'L2TP_IPSEC_PSK':
+        elif vpn_type == "L2TP_IPSEC_PSK":
             vpn_type = 1
-        elif vpn_type == 'L2TP_IPSEC_RSA':
+        elif vpn_type == "L2TP_IPSEC_RSA":
             vpn_type = 2
-        elif vpn_type == 'IPSEC_XAUTH_PSK':
+        elif vpn_type == "IPSEC_XAUTH_PSK":
             vpn_type = 3
-        elif vpn_type == 'IPSEC_XAUTH_RSA':
+        elif vpn_type == "IPSEC_XAUTH_RSA":
             vpn_type = 4
-        elif vpn_type == 'TYPE_IPSEC_HYBRID_RSA':
+        elif vpn_type == "TYPE_IPSEC_HYBRID_RSA":
             vpn_type = 5
         else:
-            raise RuntimeError('不支持的VPN类型：%s' % vpn_type)
-        
+            raise RuntimeError("不支持的VPN类型：%s" % vpn_type)
+
         timeout = 10
-        
+
         for _ in range(3):
-            if not self._device_driver.connect_vpn(vpn_type, server, username, password): return False
+            if not self._device_driver.connect_vpn(
+                vpn_type, server, username, password
+            ):
+                return False
             time0 = time.time()
             while time.time() - time0 < timeout:
-                if self._device_driver.is_vpn_connected(): return True
+                if self._device_driver.is_vpn_connected():
+                    return True
                 time.sleep(1)
         return False
-    
+
     def disconnect_vpn(self):
-        '''断开VPN
-        '''
+        """断开VPN
+        """
         return self._device_driver.disconnect_vpn()
-    
+
     def end_call(self):
-        '''挂断电话
-        '''
+        """挂断电话
+        """
         return self._device_driver.end_call()
-    
+
     def grant_all_runtime_permissions(self, package_name):
-        '''给APP授予所有运行时权限
-        '''
+        """给APP授予所有运行时权限
+        """
         return self._device_driver.grant_all_runtime_permissions(package_name)
-    
+
     def set_http_proxy(self, host, port):
-        '''设置http代理
+        """设置http代理
         
         :param host: 代理服务器地址
         :param port: 代理服务器端口
-        '''
+        """
         return self._device_driver.set_http_proxy(host, port)
-    
+
     def clear_http_proxy(self):
-        '''清除http代理
-        '''
+        """清除http代理
+        """
         return self._device_driver.set_http_proxy(None, None)
-    
+
     def register_screenshot_callback(self, callback, frame_rate=15):
-        '''注册截图回调函数
+        """注册截图回调函数
         
         :param callback: 回调函数，回调参数为PIL的Image对象
         :type  callback: function
         :param frame_rate: 期望的帧率
         :type  frame_rate: int
-        '''
+        """
         import copy
         from PIL import Image
-        if not hasattr(self, '_screenshot_callbacks'):
+
+        if not hasattr(self, "_screenshot_callbacks"):
             self._screenshot_callbacks = [callback]
             sock = self._device_driver.connect_screenshot_service()
-            sock.send(struct.pack('II', 0x3, frame_rate))
+            sock.send(struct.pack("II", 0x3, frame_rate))
+
             def recv_data(data_len):
-                data = ''
+                data = ""
                 while len(data) < data_len:
                     try:
                         buff = sock.recv(data_len - len(data))
                         if not buff:
-                            logger.warn('screenshot socket closed')
+                            logger.warn("screenshot socket closed")
                             return
                         data += buff
                     except socket.error as e:
-                        logger.warn('recv screenshot data error: %s' % e)
+                        logger.warn("recv screenshot data error: %s" % e)
                         return
                 return data
-            
+
             def screenshot_thread():
                 prev_image = None
                 max_width = max_height = 0
                 while True:
                     data = recv_data(24)
-                    if not data: return
-                    timestamp, left, top, width, height, data_len = struct.unpack('I' * 6, data)
+                    if not data:
+                        return
+                    timestamp, left, top, width, height, data_len = struct.unpack(
+                        "I" * 6, data
+                    )
                     if data_len > 0:
                         data = recv_data(data_len)
-                        assert(len(data) == data_len)
+                        assert len(data) == data_len
                         fp = BytesIO(data)
                         image = Image.open(fp)
                         # image.verify()
                         w, h = image.size
-                        if w > max_width: max_width = w
-                        if h > max_height: max_height = h
+                        if w > max_width:
+                            max_width = w
+                        if h > max_height:
+                            max_height = h
                         if w < max_width or h < max_height:
                             # 此时prev_image一定不为空
                             try:
-                                prev_image.paste(image, (left, top, left + width, top + height))
+                                prev_image.paste(
+                                    image, (left, top, left + width, top + height)
+                                )
                             except Exception as e:
-                                err_msg = 'compose image [%s]%r failed: %s' % (data_len, (left, top, width, height), e)
+                                err_msg = "compose image [%s]%r failed: %s" % (
+                                    data_len,
+                                    (left, top, width, height),
+                                    e,
+                                )
                                 raise RuntimeError(err_msg)
                         else:
                             prev_image = image
                     for callback in self._screenshot_callbacks:
                         try:
                             callback(copy.deepcopy(prev_image))
                         except:
-                            logger.exception('run callback %s failed' % callback.__name__)
+                            logger.exception(
+                                "run callback %s failed" % callback.__name__
+                            )
+
             self._screenshot_thread = threading.Thread(target=screenshot_thread)
             self._screenshot_thread.setDaemon(True)
             self._screenshot_thread.start()
         else:
-            if not callback in self._screenshot_callbacks: self._screenshot_callbacks.append(callback)
-    
+            if not callback in self._screenshot_callbacks:
+                self._screenshot_callbacks.append(callback)
+
     def unregister_screenshot_callback(self, callback):
-        '''注销截图回调函数
+        """注销截图回调函数
         
         :param callback: 回调函数
         :type  callback: function
-        '''
-        if hasattr(self, '_screenshot_callbacks') and callback in self._screenshot_callbacks:
+        """
+        if (
+            hasattr(self, "_screenshot_callbacks")
+            and callback in self._screenshot_callbacks
+        ):
             self._screenshot_callbacks.remove(callback)
- 
+
     def resolve_domain(self, domain):
-        '''解析域名
-        '''
+        """解析域名
+        """
         return self._device_driver.resolve_domain(domain)
 
     def set_radio_enabled(self, enable):
-        '''是否启用Radio
-        '''
+        """是否启用Radio
+        """
         return self._device_driver.set_radio_enabled(enable)
 
     def get_system_timezone(self):
-        '''获取当前系统时区
-        '''
-        return self.adb.get_property('persist.sys.timezone')
-
-    def set_system_timezone(self, new_timezone='Asia/Shanghai'):
-        '''修改系统时区
-        '''
+        """获取当前系统时区
+        """
+        return self.adb.get_property("persist.sys.timezone")
+
+    def set_system_timezone(self, new_timezone="Asia/Shanghai"):
+        """修改系统时区
+        """
         if self.get_system_timezone() != new_timezone:
-            self.adb.set_property('persist.sys.timezone', new_timezone)
-            
+            self.adb.set_property("persist.sys.timezone", new_timezone)
+
     def set_system_time(self, new_time=None):
-        '''设置系统时间
+        """设置系统时间
 
         :param new_time: 新时间,默认为PC上的时间,格式为: 20151001.170000
         :type  new_time: str
-        '''
+        """
         if not new_time:
             new_time = time.strftime("%Y%m%d.%H%M%S", time.localtime())
-        self.adb.run_shell_cmd('date -s %s' % new_time, self.adb.is_rooted())
+        self.adb.run_shell_cmd("date -s %s" % new_time, self.adb.is_rooted())
 
     def get_available_data_storage(self):
-        '''获取数据存储区可用空间
-        '''
-        return self._device_driver.get_available_storage('/data')
+        """获取数据存储区可用空间
+        """
+        return self._device_driver.get_available_storage("/data")
 
     def get_available_external_storage(self):
-        '''获取sdcard可用存储空间
-        '''
-        return self._device_driver.get_available_storage('/sdcard')
+        """获取sdcard可用存储空间
+        """
+        return self._device_driver.get_available_storage("/sdcard")
+
+    def dump_class_list(self, package_name, save_path, filter=None):
+        """Dump应用中的类列表
 
-if __name__ == '__main__':
+        :param package_name: 应用包名
+        :type  package_name: string
+        :param save_path: 保存路径
+        :type  save_path: string
+        :param filter: 类名过滤器
+        "type  filter: string
+        """
+        return self._device_driver.dump_class_list(package_name, save_path, filter)
+
+
+if __name__ == "__main__":
     pass
-        
-    
+
```

### Comparing `qt4a-2.3.1/qt4a/mtcontrols.py` & `qt4a-3.0.0/qt4a/mtcontrols.py`

 * *Files identical despite different names*

### Comparing `qt4a-2.3.1/qt4a/qpath.py` & `qt4a-3.0.0/qt4a/qpath.py`

 * *Files identical despite different names*

### Comparing `qt4a-2.3.1/qt4a/systemui.py` & `qt4a-3.0.0/qt4a/systemui.py`

 * *Files identical despite different names*

### Comparing `qt4a-2.3.1/qt4a.egg-info/PKG-INFO` & `qt4a-3.0.0/qt4a.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: qt4a
-Version: 2.3.1
+Version: 3.0.0
 Summary: QTA driver for Android app
 Home-page: https://github.com/Tencent/QT4A
 Author: Tencent
 License: Copyright(c)2010-2018 Tencent All Rights Reserved. 
 Project-URL: QT4A Documentation, https://qt4a.readthedocs.io/zh_CN/latest/
 Description: # QT4A
         
-        [![Build Status](https://travis-ci.org/Tencent/QT4A.svg?branch=master)](https://travis-ci.org/Tencent/QT4A) 
+        [![Build Status](https://github.com/tencent/qt4a/actions/workflows/unittest.yml/badge.svg)](https://github.com/Tencent/QT4A/actions/workflows/unittest.yml) 
         [![PyPi version](https://img.shields.io/pypi/v/qt4a.svg)](https://pypi.python.org/pypi/qt4a/) 
         [![Documentation Status](https://readthedocs.org/projects/qt4a/badge/?version=latest)](https://qt4a.readthedocs.io/zh_CN/latest/?badge=latest)
         [![GitHub tag](https://img.shields.io/github/tag/Tencent/QT4A.svg)](https://GitHub.com/Tencent/QT4A/tags/)
         [![codecov.io](https://codecov.io/github/tencent/QT4A/coverage.svg?branch=master)](https://codecov.io/github/tencent/QT4A)
         
         QT4A (Quick Test for Android) is a QTA test automation driver for Android application.
         
         ### Features
         
-         * Support most versions of Android OS from 2.3 to 8.1 
+         * Support most versions of Android OS from 4.0 to 14(armeabi-v7a、arm64-v8a、x86、x86_64)
          * Multiple devices can be used simultaneously in a test
          * Support testing multi-process application, and multiple application can be tested simultaneously
          * Support testting code obfuscated application
          * Support testing with custom controls
          * Support non-root devices
          
         QT4A should be used with [QTAF](https://github.com/Tencent/QTAF), please check it first.
@@ -35,15 +35,15 @@
         
         ------------------------------
         
         QT4A (Quick Test for Android)，基于QTA提供面向Android应用的UI测试自动化测试解决方案。
         
         ### 特性介绍
         
-        1. 支持Android 2.3 - 8.1版本
+        1. 支持Android 4.0 - 14 版本(armeabi-v7a、arm64-v8a、x86、x86_64)
         2. 支持多设备协同测试
         3. 支持跨进程、跨应用测试
         4. 支持进行过控件混淆的安装包
         5. 支持自定义（自绘）控件
         6. 支持非root设备
         
         QT4A需要和[QTAF](https://github.com/Tencent/QTAF)一起使用，请先参考QTAF的使用
```

### Comparing `qt4a-2.3.1/qt4a.egg-info/SOURCES.txt` & `qt4a-3.0.0/qt4a.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -42,33 +42,36 @@
 qt4a/androiddriver/tools/adb/linux2/adb
 qt4a/androiddriver/tools/adb/win32/AdbWinApi.dll
 qt4a/androiddriver/tools/adb/win32/AdbWinUsbApi.dll
 qt4a/androiddriver/tools/adb/win32/adb.exe
 qt4a/androiddriver/tools/arm64-v8a/droid_inject
 qt4a/androiddriver/tools/arm64-v8a/droid_inject64
 qt4a/androiddriver/tools/arm64-v8a/libandroidhook.so
-qt4a/androiddriver/tools/arm64-v8a/libandroidhook_art.so
+qt4a/androiddriver/tools/arm64-v8a/libandroidhook64.so
 qt4a/androiddriver/tools/arm64-v8a/libdexloader.so
 qt4a/androiddriver/tools/arm64-v8a/libdexloader64.so
 qt4a/androiddriver/tools/arm64-v8a/screenkit
 qt4a/androiddriver/tools/armeabi/droid_inject
-qt4a/androiddriver/tools/armeabi/libandroidhook.so
-qt4a/androiddriver/tools/armeabi/libandroidhook_art.so
 qt4a/androiddriver/tools/armeabi/libdexloader.so
 qt4a/androiddriver/tools/armeabi/screenkit
 qt4a/androiddriver/tools/armeabi-v7a/droid_inject
 qt4a/androiddriver/tools/armeabi-v7a/libandroidhook.so
-qt4a/androiddriver/tools/armeabi-v7a/libandroidhook_art.so
 qt4a/androiddriver/tools/armeabi-v7a/libdexloader.so
 qt4a/androiddriver/tools/armeabi-v7a/screenkit
 qt4a/androiddriver/tools/x86/droid_inject
 qt4a/androiddriver/tools/x86/libandroidhook.so
-qt4a/androiddriver/tools/x86/libandroidhook_art.so
 qt4a/androiddriver/tools/x86/libdexloader.so
 qt4a/androiddriver/tools/x86/screenkit
+qt4a/androiddriver/tools/x86_64/droid_inject
+qt4a/androiddriver/tools/x86_64/droid_inject64
+qt4a/androiddriver/tools/x86_64/libandroidhook.so
+qt4a/androiddriver/tools/x86_64/libandroidhook64.so
+qt4a/androiddriver/tools/x86_64/libdexloader.so
+qt4a/androiddriver/tools/x86_64/libdexloader64.so
+qt4a/androiddriver/tools/x86_64/screenkit
 qt4a/apktool/__init__.py
 qt4a/apktool/apkfile.py
 qt4a/apktool/axml.py
 qt4a/apktool/header.py
 qt4a/apktool/manifest.py
 qt4a/apktool/repack.py
 qt4a/apktool/tools/apkhelper.jar
```

### Comparing `qt4a-2.3.1/setup.py` & `qt4a-3.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `qt4a-2.3.1/test/test_andrcontrols.py` & `qt4a-3.0.0/test/test_andrcontrols.py`

 * *Files identical despite different names*

### Comparing `qt4a-2.3.1/test/test_androidapp.py` & `qt4a-3.0.0/test/test_androidapp.py`

 * *Files identical despite different names*

### Comparing `qt4a-2.3.1/test/test_device.py` & `qt4a-3.0.0/test/test_device.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,152 +1,157 @@
 # -*- coding: UTF-8 -*-
 #
 # Tencent is pleased to support the open source community by making QTA available.
 # Copyright (C) 2016THL A29 Limited, a Tencent company. All rights reserved.
-# Licensed under the BSD 3-Clause License (the "License"); you may not use this 
+# Licensed under the BSD 3-Clause License (the "License"); you may not use this
 # file except in compliance with the License. You may obtain a copy of the License at
-# 
+#
 # https://opensource.org/licenses/BSD-3-Clause
-# 
-# Unless required by applicable law or agreed to in writing, software distributed 
+#
+# Unless required by applicable law or agreed to in writing, software distributed
 # under the License is distributed on an "AS IS" basis, WITHOUT WARRANTIES OR CONDITIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 #
 
-'''device模块单元测试
-'''
+"""device模块单元测试
+"""
 
 try:
     from unittest import mock
 except:
     import mock
 import unittest
 
 import os
 from qt4a.androiddriver.adb import ADB, LocalADBBackend
 from qt4a.device import Device, LocalDeviceProvider
-from test.test_androiddriver.test_adb import mock_run_shell_cmd as mock_run_shell_cmd_adb
-from test.test_androiddriver.test_devicedriver import mock_run_shell_cmd as mock_run_shell_cmd_dev
+from test.test_androiddriver.test_adb import (
+    mock_run_shell_cmd as mock_run_shell_cmd_adb,
+)
+from test.test_androiddriver.test_devicedriver import (
+    mock_run_shell_cmd as mock_run_shell_cmd_dev,
+)
+
 
 def mock_run_shell_cmd(cmd_line, root=False, **kwds):
     try:
         return mock_run_shell_cmd_adb(cmd_line, root=root, **kwds)
     except NotImplementedError:
         return mock_run_shell_cmd_dev(cmd_line, root=root, **kwds)
-    
+
+
 class TestDevice(unittest.TestCase):
-    '''Device类测试用例
-    '''
-    
+    """Device类测试用例"""
+
     def _get_device(self):
         ADB.is_rooted = mock.Mock(return_value=False)
         ADB.run_shell_cmd = mock.Mock(side_effect=mock_run_shell_cmd)
-        adb_backend = LocalADBBackend('127.0.0.1', 'test')
+        adb_backend = LocalADBBackend("127.0.0.1", "test")
         adb = ADB(adb_backend)
-        return Device(adb)
-    
+        ADB.open_device = mock.Mock(return_value=adb)
+        return Device(adb_backend)
+
     def test_device_id(self):
         device = self._get_device()
-        self.assertEqual(device.device_id, 'test')
-    
+        self.assertEqual(device.device_id, "test")
+
     def test_device_host(self):
         device = self._get_device()
-        self.assertEqual(device.device_host, '127.0.0.1')
-    
+        self.assertEqual(device.device_host, "127.0.0.1")
+
     def test_cpu_type(self):
         device = self._get_device()
-        self.assertEqual(device.cpu_type, 'armeabi-v7a')
-    
+        self.assertEqual(device.cpu_type, "armeabi-v7a")
+
     def test_imei(self):
         device = self._get_device()
         ADB.is_rooted = mock.Mock(return_value=True)
-        self.assertEqual(device.imei, '180322023834592')
-    
+        self.assertEqual(device.imei, "180322023834592")
+
     def test_model(self):
         device = self._get_device()
-        self.assertEqual(device.model, 'Xiaomi MI 4C')
-    
+        self.assertEqual(device.model, "Xiaomi MI 4C")
+
     def test_system_version(self):
         device = self._get_device()
-        self.assertEqual(device.system_version, '5.0.2')
-    
+        self.assertEqual(device.system_version, "5.0.2")
+
     def test_sdk_version(self):
         device = self._get_device()
         self.assertEqual(device.sdk_version, 21)
-    
+
     def test_screen_size(self):
         device = self._get_device()
         self.assertEqual(device.screen_size, (800, 1280))
-    
+
     def test_screen_scale(self):
         device = self._get_device()
         self.assertEqual(device.screen_scale, 2.0)
-    
+
     def test_language(self):
         device = self._get_device()
-        self.assertEqual(device.language, 'zh')
-    
+        self.assertEqual(device.language, "zh")
+
     def test_country(self):
         device = self._get_device()
-        self.assertEqual(device.country, 'CN')
-    
+        self.assertEqual(device.country, "CN")
+
     def test_debuggable(self):
         device = self._get_device()
         self.assertEqual(device.debuggable, False)
-    
+
     def test_is_rooted(self):
         device = self._get_device()
         self.assertEqual(device.is_rooted(), False)
-    
+
     def test_is_emulator_device(self):
         device = self._get_device()
         self.assertEqual(device.is_emulator_device(), False)
-    
+
     def test_list_dir(self):
         device = self._get_device()
         ADB.is_rooted = mock.Mock(return_value=True)
-        dir_list, file_list = device.list_dir('/data/data')
+        dir_list, file_list = device.list_dir("/data/data")
         self.assertEqual(len(dir_list), 89)
         self.assertEqual(len(file_list), 0)
-        self.assertEqual(dir_list[0]['name'], 'com.android.apps.tag')
-        self.assertEqual(dir_list[0]['attr'], 'rwxr-x--x')
-    
+        self.assertEqual(dir_list[0]["name"], "com.android.apps.tag")
+        self.assertEqual(dir_list[0]["attr"], "rwxr-x--x")
+
     def test_is_file_exists(self):
         device = self._get_device()
         ADB.is_rooted = mock.Mock(return_value=True)
-        self.assertEqual(device.is_file_exists('/data/local/tmp/1.txt'), True)
+        self.assertEqual(device.is_file_exists("/data/local/tmp/1.txt"), True)
 
     def test_read_logcat(self):
         device = self._get_device()
         ADB.is_rooted = mock.Mock(return_value=True)
         adb = device.adb
         adb.start_logcat()
-        adb.insert_logcat('test', 2021, '0101', '10:59:42.899', 'I', 'test', 1, '中文')
-        adb.insert_logcat('test', 2021, '0101', '10:59:42.899', 'I', 'test', 1, '测试使用')
+        adb.insert_logcat("test", 2021, "0101", "10:59:42.899", "I", "test", 1, "中文")
+        adb.insert_logcat("test", 2021, "0101", "10:59:42.899", "I", "test", 1, "测试使用")
         print(adb.get_log(False))
-        self.assertEqual(device.read_logcat(tag='test', process_name_pattern='', pattern=''), [])
+        self.assertEqual(
+            device.read_logcat(tag="test", process_name_pattern="", pattern=""), []
+        )
 
 
 class TestLocalDeviceProvider(unittest.TestCase):
-    '''LocalDeviceProvider类测试用例
-    '''
+    """LocalDeviceProvider类测试用例"""
 
     def test_list_device(self):
-        res_device_list = ['8776fads', 'afsddsf']
+        res_device_list = ["8776fads", "afsddsf"]
         LocalADBBackend.list_device = mock.Mock(return_value=res_device_list)
         device_list = LocalDeviceProvider.list()
         self.assertEqual(len(device_list), len(res_device_list))
         self.assertEqual(set(device_list), set(res_device_list))
 
-
     def test_list_device_env(self):
-        res_device_list = ['8776fads', 'afsddsf']
-        os.environ['QT4A_AVAILABLE_DEVICES'] = 'afsddsf'
+        res_device_list = ["8776fads", "afsddsf"]
+        os.environ["QT4A_AVAILABLE_DEVICES"] = "afsddsf"
         LocalADBBackend.list_device = mock.Mock(return_value=res_device_list)
         device_list = LocalDeviceProvider.list()
-        self.assertEqual(device_list, ['afsddsf'])
+        self.assertEqual(device_list, ["afsddsf"])
+
 
-        
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
-
```

### Comparing `qt4a-2.3.1/test/test_management.py` & `qt4a-3.0.0/test/test_management.py`

 * *Files identical despite different names*

### Comparing `qt4a-2.3.1/test/test_qpath.py` & `qt4a-3.0.0/test/test_qpath.py`

 * *Files identical despite different names*

