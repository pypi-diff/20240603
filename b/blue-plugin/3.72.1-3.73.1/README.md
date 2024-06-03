# Comparing `tmp/blue_plugin-3.72.1.tar.gz` & `tmp/blue_plugin-3.73.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blue_plugin-3.72.1.tar", last modified: Mon Jun  3 05:39:25 2024, max compression
+gzip compressed data, was "blue_plugin-3.73.1.tar", last modified: Mon Jun  3 05:48:47 2024, max compression
```

## Comparing `blue_plugin-3.72.1.tar` & `blue_plugin-3.73.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 05:39:25.418501 blue_plugin-3.72.1/
--rw-r--r--   0 kamangir   (502) staff       (20)     7048 2022-09-09 01:44:55.000000 blue_plugin-3.72.1/LICENSE
--rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-20 04:48:46.000000 blue_plugin-3.72.1/MANIFEST.in
--rw-r--r--   0 kamangir   (502) staff       (20)     2044 2024-06-03 05:39:25.417902 blue_plugin-3.72.1/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)     1203 2024-06-03 05:39:17.000000 blue_plugin-3.72.1/README.md
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 05:39:25.409003 blue_plugin-3.72.1/blue_plugin/
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 05:39:25.415020 blue_plugin-3.72.1/blue_plugin/.abcli/
--rw-r--r--   0 kamangir   (502) staff       (20)      184 2024-05-26 17:21:12.000000 blue_plugin-3.72.1/blue_plugin/.abcli/abcli.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      152 2024-05-26 17:21:12.000000 blue_plugin-3.72.1/blue_plugin/.abcli/actions.sh
--rw-r--r--   0 kamangir   (502) staff       (20)       61 2024-05-26 17:21:12.000000 blue_plugin-3.72.1/blue_plugin/.abcli/aka.sh
--rwxr-xr-x   0 kamangir   (502) staff       (20)      816 2024-05-26 17:21:12.000000 blue_plugin-3.72.1/blue_plugin/.abcli/blue_plugin.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      440 2024-05-26 17:21:12.000000 blue_plugin-3.72.1/blue_plugin/.abcli/leaf.sh
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 05:39:25.415382 blue_plugin-3.72.1/blue_plugin/.abcli/node/
--rw-r--r--   0 kamangir   (502) staff       (20)     1173 2024-05-26 17:21:12.000000 blue_plugin-3.72.1/blue_plugin/.abcli/node/leaf.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      478 2024-05-26 17:21:12.000000 blue_plugin-3.72.1/blue_plugin/.abcli/node.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      376 2024-05-26 17:21:12.000000 blue_plugin-3.72.1/blue_plugin/.abcli/session.sh
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 05:39:25.416877 blue_plugin-3.72.1/blue_plugin/.abcli/tests/
--rw-r--r--   0 kamangir   (502) staff       (20)      205 2024-05-26 17:21:12.000000 blue_plugin-3.72.1/blue_plugin/.abcli/tests/thing.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      306 2024-05-26 17:21:12.000000 blue_plugin-3.72.1/blue_plugin/.abcli/tests/thing_with_args.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      162 2024-05-28 01:33:12.000000 blue_plugin-3.72.1/blue_plugin/.abcli/tests/version.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      155 2024-06-03 05:39:19.000000 blue_plugin-3.72.1/blue_plugin/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      249 2024-05-28 00:59:53.000000 blue_plugin-3.72.1/blue_plugin/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)       25 2024-04-19 01:49:55.000000 blue_plugin-3.72.1/blue_plugin/config.env
--rw-r--r--   0 kamangir   (502) staff       (20)      235 2024-04-27 21:22:01.000000 blue_plugin-3.72.1/blue_plugin/env.py
--rw-r--r--   0 kamangir   (502) staff       (20)        0 2024-02-25 23:41:15.000000 blue_plugin-3.72.1/blue_plugin/functions.py
--rw-r--r--   0 kamangir   (502) staff       (20)       92 2024-03-24 00:16:06.000000 blue_plugin-3.72.1/blue_plugin/logger.py
--rw-r--r--   0 kamangir   (502) staff       (20)       17 2022-08-20 02:33:38.000000 blue_plugin-3.72.1/blue_plugin/urls.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 05:39:25.417398 blue_plugin-3.72.1/blue_plugin.egg-info/
--rw-r--r--   0 kamangir   (502) staff       (20)     2044 2024-06-03 05:39:25.000000 blue_plugin-3.72.1/blue_plugin.egg-info/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)      749 2024-06-03 05:39:25.000000 blue_plugin-3.72.1/blue_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-06-03 05:39:25.000000 blue_plugin-3.72.1/blue_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 kamangir   (502) staff       (20)      131 2024-06-03 05:39:25.000000 blue_plugin-3.72.1/blue_plugin.egg-info/requires.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       12 2024-06-03 05:39:25.000000 blue_plugin-3.72.1/blue_plugin.egg-info/top_level.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-21 03:07:32.000000 blue_plugin-3.72.1/pyproject.toml
--rw-r--r--   0 kamangir   (502) staff       (20)      131 2024-05-20 22:39:24.000000 blue_plugin-3.72.1/requirements.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-06-03 05:39:25.418684 blue_plugin-3.72.1/setup.cfg
--rw-r--r--   0 kamangir   (502) staff       (20)      379 2024-05-26 20:32:55.000000 blue_plugin-3.72.1/setup.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 05:48:47.902047 blue_plugin-3.73.1/
+-rw-r--r--   0 kamangir   (502) staff       (20)     7048 2022-09-09 01:44:55.000000 blue_plugin-3.73.1/LICENSE
+-rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-20 04:48:46.000000 blue_plugin-3.73.1/MANIFEST.in
+-rw-r--r--   0 kamangir   (502) staff       (20)     2046 2024-06-03 05:48:47.901597 blue_plugin-3.73.1/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)     1205 2024-06-03 05:48:27.000000 blue_plugin-3.73.1/README.md
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 05:48:47.893583 blue_plugin-3.73.1/blue_plugin/
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 05:48:47.899134 blue_plugin-3.73.1/blue_plugin/.abcli/
+-rw-r--r--   0 kamangir   (502) staff       (20)      184 2024-05-26 17:21:12.000000 blue_plugin-3.73.1/blue_plugin/.abcli/abcli.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      152 2024-05-26 17:21:12.000000 blue_plugin-3.73.1/blue_plugin/.abcli/actions.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)       61 2024-05-26 17:21:12.000000 blue_plugin-3.73.1/blue_plugin/.abcli/aka.sh
+-rwxr-xr-x   0 kamangir   (502) staff       (20)      816 2024-05-26 17:21:12.000000 blue_plugin-3.73.1/blue_plugin/.abcli/blue_plugin.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      440 2024-05-26 17:21:12.000000 blue_plugin-3.73.1/blue_plugin/.abcli/leaf.sh
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 05:48:47.899435 blue_plugin-3.73.1/blue_plugin/.abcli/node/
+-rw-r--r--   0 kamangir   (502) staff       (20)     1173 2024-05-26 17:21:12.000000 blue_plugin-3.73.1/blue_plugin/.abcli/node/leaf.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      478 2024-05-26 17:21:12.000000 blue_plugin-3.73.1/blue_plugin/.abcli/node.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      376 2024-05-26 17:21:12.000000 blue_plugin-3.73.1/blue_plugin/.abcli/session.sh
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 05:48:47.900524 blue_plugin-3.73.1/blue_plugin/.abcli/tests/
+-rw-r--r--   0 kamangir   (502) staff       (20)      205 2024-05-26 17:21:12.000000 blue_plugin-3.73.1/blue_plugin/.abcli/tests/thing.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      306 2024-05-26 17:21:12.000000 blue_plugin-3.73.1/blue_plugin/.abcli/tests/thing_with_args.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      162 2024-05-28 01:33:12.000000 blue_plugin-3.73.1/blue_plugin/.abcli/tests/version.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      155 2024-06-03 05:48:42.000000 blue_plugin-3.73.1/blue_plugin/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      249 2024-05-28 00:59:53.000000 blue_plugin-3.73.1/blue_plugin/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       25 2024-04-19 01:49:55.000000 blue_plugin-3.73.1/blue_plugin/config.env
+-rw-r--r--   0 kamangir   (502) staff       (20)      235 2024-04-27 21:22:01.000000 blue_plugin-3.73.1/blue_plugin/env.py
+-rw-r--r--   0 kamangir   (502) staff       (20)        0 2024-02-25 23:41:15.000000 blue_plugin-3.73.1/blue_plugin/functions.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       92 2024-03-24 00:16:06.000000 blue_plugin-3.73.1/blue_plugin/logger.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       17 2022-08-20 02:33:38.000000 blue_plugin-3.73.1/blue_plugin/urls.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-03 05:48:47.901037 blue_plugin-3.73.1/blue_plugin.egg-info/
+-rw-r--r--   0 kamangir   (502) staff       (20)     2046 2024-06-03 05:48:47.000000 blue_plugin-3.73.1/blue_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)      749 2024-06-03 05:48:47.000000 blue_plugin-3.73.1/blue_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-06-03 05:48:47.000000 blue_plugin-3.73.1/blue_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)      131 2024-06-03 05:48:47.000000 blue_plugin-3.73.1/blue_plugin.egg-info/requires.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       12 2024-06-03 05:48:47.000000 blue_plugin-3.73.1/blue_plugin.egg-info/top_level.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-21 03:07:32.000000 blue_plugin-3.73.1/pyproject.toml
+-rw-r--r--   0 kamangir   (502) staff       (20)      131 2024-05-20 22:39:24.000000 blue_plugin-3.73.1/requirements.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-06-03 05:48:47.902126 blue_plugin-3.73.1/setup.cfg
+-rw-r--r--   0 kamangir   (502) staff       (20)      379 2024-05-26 20:32:55.000000 blue_plugin-3.73.1/setup.py
```

### Comparing `blue_plugin-3.72.1/LICENSE` & `blue_plugin-3.73.1/LICENSE`

 * *Files identical despite different names*

### Comparing `blue_plugin-3.72.1/PKG-INFO` & `blue_plugin-3.73.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blue_plugin
-Version: 3.72.1
+Version: 3.73.1
 Summary: 🌀 a git template for an awesome-bash-cli plugin.
 Home-page: https://github.com/kamangir/blue-plugin
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
@@ -35,21 +35,21 @@
 - [pytest](https://docs.pytest.org/).
 - [pylint](https://pypi.org/project/pylint/).
 - a python package.
 - [pypi](https://pypi.org/).
 - a bash interface.
 - bash testing.
 
-# installation
+## installation
 
 ```bash
 pip install blue-plugin
 ```
 
-# creating a blue-plugin
+## creating a blue-plugin
 
 create a new repository from [this repo](https://github.com/kamangir/blue-plugin), then replace `<plugin-name>` with the name of the plugin and run these commands,
 
 ```bash
 @git clone <plugin-name> cd
 source transform.sh
```

### Comparing `blue_plugin-3.72.1/README.md` & `blue_plugin-3.73.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 - [pytest](https://docs.pytest.org/).
 - [pylint](https://pypi.org/project/pylint/).
 - a python package.
 - [pypi](https://pypi.org/).
 - a bash interface.
 - bash testing.
 
-# installation
+## installation
 
 ```bash
 pip install blue-plugin
 ```
 
-# creating a blue-plugin
+## creating a blue-plugin
 
 create a new repository from [this repo](https://github.com/kamangir/blue-plugin), then replace `<plugin-name>` with the name of the plugin and run these commands,
 
 ```bash
 @git clone <plugin-name> cd
 source transform.sh
```

### Comparing `blue_plugin-3.72.1/blue_plugin/.abcli/blue_plugin.sh` & `blue_plugin-3.73.1/blue_plugin/.abcli/blue_plugin.sh`

 * *Files identical despite different names*

### Comparing `blue_plugin-3.72.1/blue_plugin/.abcli/node/leaf.sh` & `blue_plugin-3.73.1/blue_plugin/.abcli/node/leaf.sh`

 * *Files identical despite different names*

### Comparing `blue_plugin-3.72.1/blue_plugin.egg-info/PKG-INFO` & `blue_plugin-3.73.1/blue_plugin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blue_plugin
-Version: 3.72.1
+Version: 3.73.1
 Summary: 🌀 a git template for an awesome-bash-cli plugin.
 Home-page: https://github.com/kamangir/blue-plugin
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
@@ -35,21 +35,21 @@
 - [pytest](https://docs.pytest.org/).
 - [pylint](https://pypi.org/project/pylint/).
 - a python package.
 - [pypi](https://pypi.org/).
 - a bash interface.
 - bash testing.
 
-# installation
+## installation
 
 ```bash
 pip install blue-plugin
 ```
 
-# creating a blue-plugin
+## creating a blue-plugin
 
 create a new repository from [this repo](https://github.com/kamangir/blue-plugin), then replace `<plugin-name>` with the name of the plugin and run these commands,
 
 ```bash
 @git clone <plugin-name> cd
 source transform.sh
```

### Comparing `blue_plugin-3.72.1/blue_plugin.egg-info/SOURCES.txt` & `blue_plugin-3.73.1/blue_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

