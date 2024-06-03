# Comparing `tmp/pyhidra-1.1.0.tar.gz` & `tmp/pyhidra-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhidra-1.1.0.tar", last modified: Wed Apr 24 23:28:12 2024, max compression
+gzip compressed data, was "pyhidra-1.2.0.tar", last modified: Mon Jun  3 15:17:53 2024, max compression
```

## Comparing `pyhidra-1.1.0.tar` & `pyhidra-1.2.0.tar`

### file list

```diff
@@ -1,66 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:28:12.428518 pyhidra-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-24 23:27:58.000000 pyhidra-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-24 23:27:58.000000 pyhidra-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9354 2024-04-24 23:28:12.428518 pyhidra-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8359 2024-04-24 23:27:58.000000 pyhidra-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:28:12.420518 pyhidra-1.1.0/pyhidra/
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7261 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/converters.py
--rw-r--r--   0 runner    (1001) docker     (127)    13977 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/gui.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/install_desktop.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/install_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:28:12.420518 pyhidra-1.1.0/pyhidra/java/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/java/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:28:12.424518 pyhidra-1.1.0/pyhidra/java/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)     4101 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/java/plugin/PyScriptProvider.java
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/java/plugin/PyhidraPlugin.java
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/java/plugin/PythonFieldExposer.java
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/java/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/java/plugin/completions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:28:12.424518 pyhidra-1.1.0/pyhidra/java/plugin/ghidra_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/java/plugin/ghidra_scripts/PyhidraBasics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:28:12.424518 pyhidra-1.1.0/pyhidra/java/plugin/interpreter/
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/java/plugin/interpreter/CancelAction.java
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/java/plugin/interpreter/InterpreterGhidraScript.java
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/java/plugin/interpreter/InterpreterTaskMonitor.java
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/java/plugin/interpreter/PyhidraInterpreterConnection.java
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/java/plugin/interpreter/RestartAction.java
--rw-r--r--   0 runner    (1001) docker     (127)     8054 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/java/plugin/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:28:12.428518 pyhidra-1.1.0/pyhidra/java/property/
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/java/property/AbstractJavaProperty.java
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/java/property/BooleanJavaProperty.java
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/java/property/ByteJavaProperty.java
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/java/property/CharacterJavaProperty.java
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/java/property/DoubleJavaProperty.java
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/java/property/FloatJavaProperty.java
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/java/property/IntegerJavaProperty.java
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/java/property/JavaProperty.java
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/java/property/JavaPropertyFactory.java
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/java/property/LongJavaProperty.java
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/java/property/ObjectJavaProperty.java
--rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/java/property/PropertyUtils.java
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/java/property/ShortJavaProperty.java
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/javac.py
--rw-r--r--   0 runner    (1001) docker     (127)    20899 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/launcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/linux_shortcut.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     8028 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/script.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/uninstall_desktop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/uninstall_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-04-24 23:27:58.000000 pyhidra-1.1.0/pyhidra/win_shortcut.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:28:12.428518 pyhidra-1.1.0/pyhidra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9354 2024-04-24 23:28:12.000000 pyhidra-1.1.0/pyhidra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-24 23:28:12.000000 pyhidra-1.1.0/pyhidra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 23:28:12.000000 pyhidra-1.1.0/pyhidra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-24 23:28:12.000000 pyhidra-1.1.0/pyhidra.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 23:28:12.000000 pyhidra-1.1.0/pyhidra.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-24 23:28:12.000000 pyhidra-1.1.0/pyhidra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-24 23:28:12.000000 pyhidra-1.1.0/pyhidra.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-24 23:28:12.428518 pyhidra-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-24 23:27:58.000000 pyhidra-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:28:12.428518 pyhidra-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-04-24 23:27:58.000000 pyhidra-1.1.0/tests/test_argparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6893 2024-04-24 23:27:58.000000 pyhidra-1.1.0/tests/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:17:53.815779 pyhidra-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-06-03 15:17:36.000000 pyhidra-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-06-03 15:17:36.000000 pyhidra-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9511 2024-06-03 15:17:53.815779 pyhidra-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8564 2024-06-03 15:17:36.000000 pyhidra-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:17:53.791779 pyhidra-1.2.0/pyhidra/
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-06-03 15:17:36.000000 pyhidra-1.2.0/pyhidra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7261 2024-06-03 15:17:36.000000 pyhidra-1.2.0/pyhidra/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-06-03 15:17:36.000000 pyhidra-1.2.0/pyhidra/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13977 2024-06-03 15:17:36.000000 pyhidra-1.2.0/pyhidra/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-06-03 15:17:36.000000 pyhidra-1.2.0/pyhidra/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-06-03 15:17:36.000000 pyhidra-1.2.0/pyhidra/install_desktop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-06-03 15:17:36.000000 pyhidra-1.2.0/pyhidra/install_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:17:53.795779 pyhidra-1.2.0/pyhidra/java/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:17:36.000000 pyhidra-1.2.0/pyhidra/java/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:17:53.799779 pyhidra-1.2.0/pyhidra/java/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)     4101 2024-06-03 15:17:36.000000 pyhidra-1.2.0/pyhidra/java/plugin/PyScriptProvider.java
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-06-03 15:17:36.000000 pyhidra-1.2.0/pyhidra/java/plugin/PyhidraPlugin.java
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-06-03 15:17:36.000000 pyhidra-1.2.0/pyhidra/java/plugin/PythonFieldExposer.java
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-06-03 15:17:36.000000 pyhidra-1.2.0/pyhidra/java/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-06-03 15:17:36.000000 pyhidra-1.2.0/pyhidra/java/plugin/completions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:17:53.803779 pyhidra-1.2.0/pyhidra/java/plugin/ghidra_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-06-03 15:17:36.000000 pyhidra-1.2.0/pyhidra/java/plugin/ghidra_scripts/PyhidraBasics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:17:53.807779 pyhidra-1.2.0/pyhidra/java/plugin/interpreter/
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-06-03 15:17:36.000000 pyhidra-1.2.0/pyhidra/java/plugin/interpreter/CancelAction.java
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-06-03 15:17:36.000000 pyhidra-1.2.0/pyhidra/java/plugin/interpreter/InterpreterGhidraScript.java
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-06-03 15:17:36.000000 pyhidra-1.2.0/pyhidra/java/plugin/interpreter/InterpreterTaskMonitor.java
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-06-03 15:17:36.000000 pyhidra-1.2.0/pyhidra/java/plugin/interpreter/PyhidraInterpreterConnection.java
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-06-03 15:17:36.000000 pyhidra-1.2.0/pyhidra/java/plugin/interpreter/RestartAction.java
+-rw-r--r--   0 runner    (1001) docker     (127)     8187 2024-06-03 15:17:36.000000 pyhidra-1.2.0/pyhidra/java/plugin/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:17:53.815779 pyhidra-1.2.0/pyhidra/java/property/
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-06-03 15:17:36.000000 pyhidra-1.2.0/pyhidra/java/property/AbstractJavaProperty.java
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-06-03 15:17:36.000000 pyhidra-1.2.0/pyhidra/java/property/BooleanJavaProperty.java
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-06-03 15:17:36.000000 pyhidra-1.2.0/pyhidra/java/property/ByteJavaProperty.java
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-06-03 15:17:36.000000 pyhidra-1.2.0/pyhidra/java/property/CharacterJavaProperty.java
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-06-03 15:17:36.000000 pyhidra-1.2.0/pyhidra/java/property/DoubleJavaProperty.java
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-06-03 15:17:36.000000 pyhidra-1.2.0/pyhidra/java/property/FloatJavaProperty.java
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-06-03 15:17:36.000000 pyhidra-1.2.0/pyhidra/java/property/IntegerJavaProperty.java
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-06-03 15:17:36.000000 pyhidra-1.2.0/pyhidra/java/property/JavaProperty.java
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-06-03 15:17:36.000000 pyhidra-1.2.0/pyhidra/java/property/JavaPropertyFactory.java
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-06-03 15:17:36.000000 pyhidra-1.2.0/pyhidra/java/property/LongJavaProperty.java
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-06-03 15:17:36.000000 pyhidra-1.2.0/pyhidra/java/property/ObjectJavaProperty.java
+-rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-06-03 15:17:36.000000 pyhidra-1.2.0/pyhidra/java/property/PropertyUtils.java
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-06-03 15:17:36.000000 pyhidra-1.2.0/pyhidra/java/property/ShortJavaProperty.java
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-06-03 15:17:36.000000 pyhidra-1.2.0/pyhidra/javac.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21707 2024-06-03 15:17:36.000000 pyhidra-1.2.0/pyhidra/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-06-03 15:17:36.000000 pyhidra-1.2.0/pyhidra/linux_shortcut.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5188 2024-06-03 15:17:36.000000 pyhidra-1.2.0/pyhidra/mac_shortcut.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-06-03 15:17:36.000000 pyhidra-1.2.0/pyhidra/properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8534 2024-06-03 15:17:36.000000 pyhidra-1.2.0/pyhidra/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-06-03 15:17:36.000000 pyhidra-1.2.0/pyhidra/uninstall_desktop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-06-03 15:17:36.000000 pyhidra-1.2.0/pyhidra/uninstall_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-06-03 15:17:36.000000 pyhidra-1.2.0/pyhidra/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-06-03 15:17:36.000000 pyhidra-1.2.0/pyhidra/win_shortcut.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:17:53.815779 pyhidra-1.2.0/pyhidra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9511 2024-06-03 15:17:53.000000 pyhidra-1.2.0/pyhidra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-06-03 15:17:53.000000 pyhidra-1.2.0/pyhidra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 15:17:53.000000 pyhidra-1.2.0/pyhidra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-06-03 15:17:53.000000 pyhidra-1.2.0/pyhidra.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 15:17:53.000000 pyhidra-1.2.0/pyhidra.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-06-03 15:17:53.000000 pyhidra-1.2.0/pyhidra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-06-03 15:17:53.000000 pyhidra-1.2.0/pyhidra.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-06-03 15:17:53.819779 pyhidra-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-06-03 15:17:36.000000 pyhidra-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:17:53.815779 pyhidra-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-06-03 15:17:36.000000 pyhidra-1.2.0/tests/test_argparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6893 2024-06-03 15:17:36.000000 pyhidra-1.2.0/tests/test_core.py
```

### Comparing `pyhidra-1.1.0/LICENSE` & `pyhidra-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhidra-1.1.0/PKG-INFO` & `pyhidra-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhidra
-Version: 1.1.0
+Version: 1.2.0
 Summary: Native CPython for Ghidra
 Home-page: https://github.com/Defense-Cyber-Crime-Center/pyhidra
 Author: DC3
 Author-email: dcci@dc3.mil
 License: MIT
 Keywords: ghidra
 Platform: any
@@ -16,15 +16,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Jpype1>=1.3.0; python_version < "3.12"
-Requires-Dist: pyobjc; sys_platform == "darwin"
 Requires-Dist: Jpype1>=1.5.0; python_version >= "3.12"
 Provides-Extra: testing
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-datadir; extra == "testing"
 
 # pyhidra
 
@@ -53,22 +52,25 @@
 4. From the menu in the image below select `configure` under `Experimental`.
  ![](https://raw.githubusercontent.com/Defense-Cyber-Crime-Center/pyhidra/master/images/image-20220111154029764.png)
 5. Check and enable Pyhidra as seen in the image below.
  ![](https://raw.githubusercontent.com/Defense-Cyber-Crime-Center/pyhidra/master/images/image-20220111154120531.png)
 
 ### Desktop Entry
 
-If on linux or windows, a desktop entry can be created to launch an instance of Ghidra with pyhidra attached.
+If on linux, mac or windows, a desktop entry can be created to launch an instance of Ghidra with pyhidra attached.
+When this script is run from a virtual environment (ie. venv), pyhidra will be started in this virtual environment
+when launched.
 
 ```console
 python -m pyhidra.install_desktop
 ```
 
 On windows, this will install a shortcut file on the user's desktop. On linux, this will create an entry 
-that can be found in the applications launcher.
+that can be found in the applications launcher. On mac this will create an entry that can be found in 
+the Launchpad.
 
 
 To remove, run the following:
 
 ```console
 python -m pyhidra.uninstall_desktop
 ```
```

### Comparing `pyhidra-1.1.0/README.md` & `pyhidra-1.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -25,22 +25,25 @@
 4. From the menu in the image below select `configure` under `Experimental`.
  ![](https://raw.githubusercontent.com/Defense-Cyber-Crime-Center/pyhidra/master/images/image-20220111154029764.png)
 5. Check and enable Pyhidra as seen in the image below.
  ![](https://raw.githubusercontent.com/Defense-Cyber-Crime-Center/pyhidra/master/images/image-20220111154120531.png)
 
 ### Desktop Entry
 
-If on linux or windows, a desktop entry can be created to launch an instance of Ghidra with pyhidra attached.
+If on linux, mac or windows, a desktop entry can be created to launch an instance of Ghidra with pyhidra attached.
+When this script is run from a virtual environment (ie. venv), pyhidra will be started in this virtual environment
+when launched.
 
 ```console
 python -m pyhidra.install_desktop
 ```
 
 On windows, this will install a shortcut file on the user's desktop. On linux, this will create an entry 
-that can be found in the applications launcher.
+that can be found in the applications launcher. On mac this will create an entry that can be found in 
+the Launchpad.
 
 
 To remove, run the following:
 
 ```console
 python -m pyhidra.uninstall_desktop
 ```
```

### Comparing `pyhidra-1.1.0/pyhidra/__main__.py` & `pyhidra-1.2.0/pyhidra/__main__.py`

 * *Files identical despite different names*

### Comparing `pyhidra-1.1.0/pyhidra/core.py` & `pyhidra-1.2.0/pyhidra/core.py`

 * *Files identical despite different names*

### Comparing `pyhidra-1.1.0/pyhidra/gui.py` & `pyhidra-1.2.0/pyhidra/gui.py`

 * *Files identical despite different names*

### Comparing `pyhidra-1.1.0/pyhidra/install_desktop.py` & `pyhidra-1.2.0/pyhidra/install_desktop.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,11 +22,13 @@
     )
     args = parser.parse_args()
 
     if sys.platform == "win32":
         from pyhidra.win_shortcut import create_shortcut
     elif sys.platform == "linux":
         from pyhidra.linux_shortcut import create_shortcut
+    elif sys.platform == "darwin":
+        from pyhidra.mac_shortcut import create_shortcut
     else:
         sys.exit("Unsupported platform")
 
     create_shortcut(args.install_dir)
```

### Comparing `pyhidra-1.1.0/pyhidra/install_plugins.py` & `pyhidra-1.2.0/pyhidra/install_plugins.py`

 * *Files identical despite different names*

### Comparing `pyhidra-1.1.0/pyhidra/java/plugin/PyScriptProvider.java` & `pyhidra-1.2.0/pyhidra/java/plugin/PyScriptProvider.java`

 * *Files identical despite different names*

### Comparing `pyhidra-1.1.0/pyhidra/java/plugin/PyhidraPlugin.java` & `pyhidra-1.2.0/pyhidra/java/plugin/PyhidraPlugin.java`

 * *Files identical despite different names*

### Comparing `pyhidra-1.1.0/pyhidra/java/plugin/PythonFieldExposer.java` & `pyhidra-1.2.0/pyhidra/java/plugin/PythonFieldExposer.java`

 * *Files identical despite different names*

### Comparing `pyhidra-1.1.0/pyhidra/java/plugin/ghidra_scripts/PyhidraBasics.py` & `pyhidra-1.2.0/pyhidra/java/plugin/ghidra_scripts/PyhidraBasics.py`

 * *Files identical despite different names*

### Comparing `pyhidra-1.1.0/pyhidra/java/plugin/interpreter/CancelAction.java` & `pyhidra-1.2.0/pyhidra/java/plugin/interpreter/CancelAction.java`

 * *Files identical despite different names*

### Comparing `pyhidra-1.1.0/pyhidra/java/plugin/interpreter/InterpreterGhidraScript.java` & `pyhidra-1.2.0/pyhidra/java/plugin/interpreter/InterpreterGhidraScript.java`

 * *Files identical despite different names*

### Comparing `pyhidra-1.1.0/pyhidra/java/plugin/interpreter/InterpreterTaskMonitor.java` & `pyhidra-1.2.0/pyhidra/java/plugin/interpreter/InterpreterTaskMonitor.java`

 * *Files identical despite different names*

### Comparing `pyhidra-1.1.0/pyhidra/java/plugin/interpreter/PyhidraInterpreterConnection.java` & `pyhidra-1.2.0/pyhidra/java/plugin/interpreter/PyhidraInterpreterConnection.java`

 * *Files identical despite different names*

### Comparing `pyhidra-1.1.0/pyhidra/java/plugin/interpreter/RestartAction.java` & `pyhidra-1.2.0/pyhidra/java/plugin/interpreter/RestartAction.java`

 * *Files identical despite different names*

### Comparing `pyhidra-1.1.0/pyhidra/java/plugin/plugin.py` & `pyhidra-1.2.0/pyhidra/java/plugin/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import contextlib
 import ctypes
-import itertools
 import logging
-import rlcompleter
+import re
 import sys
 import threading
 from code import InteractiveConsole
 
-from ghidra.app.plugin.core.console import CodeCompletion
 from ghidra.app.plugin.core.interpreter import InterpreterConsole, InterpreterPanelService
 from ghidra.framework import Application
 from java.io import BufferedReader, InputStreamReader, PushbackReader
 from java.lang import ClassLoader, Runnable, String
 from java.util import Collections
 from java.util.function import Consumer
 from jpype import JClass, JImplements, JOverride
@@ -166,14 +164,16 @@
 
 
 @JImplements("dc3.pyhidra.plugin.interpreter.PyhidraInterpreterConnection")
 class PyPhidraPlugin:
     """
     The Python side PyhidraPlugin
     """
+    
+    _WORD_PATTERN = re.compile(r".*?([\w\.]+)\Z") # get the last word, including '.', from the right
 
     def __init__(self, plugin):
         if hasattr(self, '_plugin'):
             # this gets entered twice for some reason
             return
         self._plugin = plugin
         self._actions = None
@@ -220,14 +220,17 @@
         try:
             if len(args) == 2:
                 line, pos = args
                 line = line[:pos]
             else:
                 # older versions of Ghidra don't have the `end` argument.
                 line, = args
+            match = self._WORD_PATTERN.match(line)
+            if match:
+                line = match.group(1)
             return self.completer.get_completions(line)
         except Exception as e:
             if not self._logged_completions_change:
                 self._logged_completions_change = True
                 logger.exception(e, exc_info=e)
             return Collections.emptyList()
```

### Comparing `pyhidra-1.1.0/pyhidra/java/property/AbstractJavaProperty.java` & `pyhidra-1.2.0/pyhidra/java/property/AbstractJavaProperty.java`

 * *Files identical despite different names*

### Comparing `pyhidra-1.1.0/pyhidra/java/property/JavaPropertyFactory.java` & `pyhidra-1.2.0/pyhidra/java/property/JavaPropertyFactory.java`

 * *Files identical despite different names*

### Comparing `pyhidra-1.1.0/pyhidra/java/property/PropertyUtils.java` & `pyhidra-1.2.0/pyhidra/java/property/PropertyUtils.java`

 * *Files identical despite different names*

### Comparing `pyhidra-1.1.0/pyhidra/javac.py` & `pyhidra-1.2.0/pyhidra/javac.py`

 * *Files identical despite different names*

### Comparing `pyhidra-1.1.0/pyhidra/launcher.py` & `pyhidra-1.2.0/pyhidra/launcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import contextlib
+import ctypes
+import ctypes.util
 import importlib.metadata
 import inspect
 import logging
 import os
 import platform
 import re
 import shutil
@@ -117,14 +119,16 @@
         self.vm_args = self._jvm_args(self._install_dir)
         self.args = []
         self.app_info = ApplicationInfo.from_file(ghidra_dir / "application.properties")
 
     @classmethod
     def _jvm_args(cls, install_dir: Path) -> List[str]:
         suffix = "_" + platform.system().upper()
+        if suffix == "_DARWIN":
+            suffix = "_MACOS"
         option_pattern: re.Pattern = re.compile(fr"VMARGS(?:{suffix})?=(.+)")
         properties = []
 
         launch_properties = install_dir / "support" / "launch.properties"
 
         with open(launch_properties, "r", encoding='utf-8') as fd:
             # this file is small so just read it at once
@@ -550,25 +554,41 @@
         from java.lang import Thread
         for t in Thread.getAllStackTraces().keySet():
             if t.getName() == name:
                 return t
         return None
 
     def _launch(self):
-        import ctypes
         from ghidra import Ghidra
         from java.lang import Runtime, Thread
 
         if sys.platform == "win32":
             appid = ctypes.c_wchar_p(self.app_info.name)
             ctypes.windll.shell32.SetCurrentProcessExplicitAppUserModelID(appid)
 
         stdout = _PyhidraStdOut(sys.stdout)
         stderr = _PyhidraStdOut(sys.stderr)
         with contextlib.redirect_stdout(stdout), contextlib.redirect_stderr(stderr):
-            jpype.setupGuiEnvironment(lambda: Ghidra.main(["ghidra.GhidraRun", *self.args]))
+            Thread(lambda: Ghidra.main(["ghidra.GhidraRun", *self.args])).start()
             is_exiting = threading.Event()
             Runtime.getRuntime().addShutdownHook(Thread(is_exiting.set))
-            try:
-                is_exiting.wait()
-            finally:
-                jpype.shutdownGuiEnvironment()
+            if sys.platform == "darwin":
+                _run_mac_app()
+            is_exiting.wait()
+
+
+def _run_mac_app():
+    # this runs the main event loop
+    # it is required for the GUI to show up
+    objc = ctypes.cdll.LoadLibrary(ctypes.util.find_library("libobjc"))
+    ctypes.cdll.LoadLibrary(ctypes.util.find_library("AppKit")) # required
+    msgSend = objc.objc_msgSend
+    msgSend.restype = ctypes.c_void_p
+    msgSend.argtypes = [ctypes.c_void_p, ctypes.c_void_p]
+    registerName = objc.sel_registerName
+    registerName.restype = ctypes.c_void_p
+    registerName.argtypes = [ctypes.c_char_p]
+    getClass = objc.objc_getClass
+    getClass.restype = ctypes.c_void_p
+    NSApplication = getClass(b"NSApplication")
+    sharedApplication = msgSend(NSApplication, registerName(b"sharedApplication"))
+    msgSend(sharedApplication, registerName(b"run"))
```

### Comparing `pyhidra-1.1.0/pyhidra/linux_shortcut.py` & `pyhidra-1.2.0/pyhidra/linux_shortcut.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,28 +35,33 @@
     return png_path
 
 
 def create_shortcut(install_dir: Path = None):
     """Install a desktop entry on Linux machine."""
     pyhidra_exec = Path(sysconfig.get_path("scripts")) / "pyhidra"
     if not pyhidra_exec.exists():
+        # User install
+        pyhidra_exec = Path(sysconfig.get_path("scripts", "posix_user")) / "pyhidra"
+    if not pyhidra_exec.exists():
         sys.exit("pyhidra executable is not installed.")
 
-    command = [str(pyhidra_exec), "--gui"]
     if install_dir:
-        command += ["--install-dir", str(install_dir.expanduser())]
+        pass
     elif install_dir := os.environ.get("GHIDRA_INSTALL_DIR"):
         install_dir = Path(install_dir)
     else:
         sys.exit(
             "Unable to determine Ghidra installation directory. "
             "Please set the GHIDRA_INSTALL_DIR environment variable."
         )
+    
+    command = [str(pyhidra_exec), "--gui", "--install-dir", str(install_dir.expanduser())]
 
     icon = extract_png(install_dir)
+    desktop_path.parent.mkdir(parents=True, exist_ok=True)
     desktop_path.write_text(desktop_entry.format(icon=icon, exec=shlex.join(command)))
     print(f"Installed {desktop_path}")
 
 
 def remove_shortcut():
     if desktop_path.exists():
         desktop_path.unlink()
```

### Comparing `pyhidra-1.1.0/pyhidra/properties.py` & `pyhidra-1.2.0/pyhidra/properties.py`

 * *Files identical despite different names*

### Comparing `pyhidra-1.1.0/pyhidra/script.py` & `pyhidra-1.2.0/pyhidra/script.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,24 +13,33 @@
 
 _NO_ATTRIBUTE = object()
 
 _headless_interpreter = None
 
 
 class _StaticMap(dict):
+    # this is a special view of the PyGhidraScript for use with rlcompleter
 
     __slots__ = ('script',)
 
     def __init__(self, script: "PyGhidraScript"):
         super().__init__()
         self.script = script
 
     def __getitem__(self, key):
         res = self.get(key, _NO_ATTRIBUTE)
         if res is not _NO_ATTRIBUTE:
+            if isinstance(res, property):
+                # rlcompleter is attempting to use a property getter on the interpreter script
+                # allow the property magic to take place
+                # this is necessary for completions on currentAddress, currentProgram, etc.
+                try:
+                    return getattr(self.script, key)
+                except AttributeError:
+                    return res
             return res
         raise KeyError(key)
 
     def get(self, key, default=None):
         res = self.script.get_static(key)
         return res if res is not _NO_ATTRIBUTE else default
```

### Comparing `pyhidra-1.1.0/pyhidra/uninstall_plugin.py` & `pyhidra-1.2.0/pyhidra/uninstall_plugin.py`

 * *Files identical despite different names*

### Comparing `pyhidra-1.1.0/pyhidra/version.py` & `pyhidra-1.2.0/pyhidra/version.py`

 * *Files identical despite different names*

### Comparing `pyhidra-1.1.0/pyhidra/win_shortcut.py` & `pyhidra-1.2.0/pyhidra/win_shortcut.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     WINFUNCTYPE = ctypes.WINFUNCTYPE
     _CoCreateInstance = ctypes.oledll.ole32.CoCreateInstance
     _QueryInterface = WINFUNCTYPE(ctypes.HRESULT, _GUID, ctypes.c_void_p)(0, "QueryInterface")
     _Release = WINFUNCTYPE(ctypes.HRESULT)(2, "Release")
     _Save = WINFUNCTYPE(ctypes.HRESULT, ctypes.c_wchar_p, ctypes.wintypes.BOOL)(6, "Save")
     _SetPath = WINFUNCTYPE(ctypes.HRESULT, ctypes.c_wchar_p)(20, "SetPath")
     _SetDescription = WINFUNCTYPE(ctypes.HRESULT, ctypes.c_wchar_p)(7, "SetDescription")
-    _SetIconLocation = WINFUNCTYPE(ctypes.HRESULT, ctypes.c_wchar_p)(17, "SetIconLocation")
+    _SetIconLocation = WINFUNCTYPE(ctypes.HRESULT, ctypes.c_wchar_p, ctypes.c_int)(17, "SetIconLocation")
     _SetValue = WINFUNCTYPE(ctypes.HRESULT, ctypes.c_void_p, ctypes.c_void_p)(6, "SetValue")
 
     link = str(link)
     target = Path(sysconfig.get_path("scripts")) / "pyhidraw.exe"
     icon = str(launcher.install_dir / "support" / "ghidra.ico")
     p_link = ctypes.c_void_p()
     p_file = ctypes.c_void_p()
@@ -63,15 +63,15 @@
     p_app_id = ctypes.wintypes.LPCWSTR(_APP_ID)
     ctypes.oledll.ole32.CoInitializeEx(None, _COINIT_APARTMENTTHREADED | _COINIT_DISABLE_OLE1DDE)
     try:
         ref = ctypes.byref(p_link)
         _CoCreateInstance(_CLSID_ShellLink, None, _CLSCTX_INPROC_SERVER, _IID_IShellLinkW, ref)
         _SetPath(p_link, ctypes.c_wchar_p(str(target)))
         _SetDescription(p_link, p_app_id)
-        _SetIconLocation(p_link, ctypes.c_wchar_p(icon))
+        _SetIconLocation(p_link, ctypes.c_wchar_p(icon), 0)
         _QueryInterface(p_link, _IID_IPropertyStore, ctypes.byref(p_store))
         value = _PropertyVariant.pack(_VT_LPWSTR, ctypes.cast(p_app_id, ctypes.c_void_p).value)
         value = (ctypes.c_byte * len(value))(*value)
         _SetValue(p_store, ctypes.byref(_AppUserModelId), ctypes.byref(value))
         _QueryInterface(p_link, _IID_IPersistFile, ctypes.byref(p_file))
         _Save(p_file, ctypes.c_wchar_p(link), True)
     finally:
```

### Comparing `pyhidra-1.1.0/pyhidra.egg-info/PKG-INFO` & `pyhidra-1.2.0/pyhidra.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhidra
-Version: 1.1.0
+Version: 1.2.0
 Summary: Native CPython for Ghidra
 Home-page: https://github.com/Defense-Cyber-Crime-Center/pyhidra
 Author: DC3
 Author-email: dcci@dc3.mil
 License: MIT
 Keywords: ghidra
 Platform: any
@@ -16,15 +16,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Jpype1>=1.3.0; python_version < "3.12"
-Requires-Dist: pyobjc; sys_platform == "darwin"
 Requires-Dist: Jpype1>=1.5.0; python_version >= "3.12"
 Provides-Extra: testing
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-datadir; extra == "testing"
 
 # pyhidra
 
@@ -53,22 +52,25 @@
 4. From the menu in the image below select `configure` under `Experimental`.
  ![](https://raw.githubusercontent.com/Defense-Cyber-Crime-Center/pyhidra/master/images/image-20220111154029764.png)
 5. Check and enable Pyhidra as seen in the image below.
  ![](https://raw.githubusercontent.com/Defense-Cyber-Crime-Center/pyhidra/master/images/image-20220111154120531.png)
 
 ### Desktop Entry
 
-If on linux or windows, a desktop entry can be created to launch an instance of Ghidra with pyhidra attached.
+If on linux, mac or windows, a desktop entry can be created to launch an instance of Ghidra with pyhidra attached.
+When this script is run from a virtual environment (ie. venv), pyhidra will be started in this virtual environment
+when launched.
 
 ```console
 python -m pyhidra.install_desktop
 ```
 
 On windows, this will install a shortcut file on the user's desktop. On linux, this will create an entry 
-that can be found in the applications launcher.
+that can be found in the applications launcher. On mac this will create an entry that can be found in 
+the Launchpad.
 
 
 To remove, run the following:
 
 ```console
 python -m pyhidra.uninstall_desktop
 ```
```

### Comparing `pyhidra-1.1.0/pyhidra.egg-info/SOURCES.txt` & `pyhidra-1.2.0/pyhidra.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 pyhidra/core.py
 pyhidra/gui.py
 pyhidra/install_desktop.py
 pyhidra/install_plugins.py
 pyhidra/javac.py
 pyhidra/launcher.py
 pyhidra/linux_shortcut.py
+pyhidra/mac_shortcut.py
 pyhidra/properties.py
 pyhidra/script.py
 pyhidra/uninstall_desktop.py
 pyhidra/uninstall_plugin.py
 pyhidra/version.py
 pyhidra/win_shortcut.py
 pyhidra.egg-info/PKG-INFO
```

### Comparing `pyhidra-1.1.0/setup.cfg` & `pyhidra-1.2.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 [options]
 python_requires = >= 3.9
 packages = find:
 zip_safe = False
 include_package_data = True
 install_requires = 
 	Jpype1>=1.3.0; python_version < '3.12'
-	pyobjc; sys_platform == "darwin"
 	Jpype1>=1.5.0; python_version >= '3.12'
 
 [options.entry_points]
 console_scripts = 
 	pyhidra = pyhidra.__main__:main
 gui_scripts = 
 	pyhidraw = pyhidra.gui:_gui
```

### Comparing `pyhidra-1.1.0/tests/test_argparser.py` & `pyhidra-1.2.0/tests/test_argparser.py`

 * *Files identical despite different names*

### Comparing `pyhidra-1.1.0/tests/test_core.py` & `pyhidra-1.2.0/tests/test_core.py`

 * *Files identical despite different names*

