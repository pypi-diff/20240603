# Comparing `tmp/xeus_python_shell-0.6.2.tar.gz` & `tmp/xeus_python_shell-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xeus_python_shell-0.6.2.tar", last modified: Fri May 31 13:32:23 2024, max compression
+gzip compressed data, was "xeus_python_shell-0.6.3.tar", last modified: Mon Jun  3 07:15:18 2024, max compression
```

## Comparing `xeus_python_shell-0.6.2.tar` & `xeus_python_shell-0.6.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2024-05-31 13:32:23.579568 xeus_python_shell-0.6.2/
--rw-r--r--   0 martin    (1000) martin    (1000)     1518 2024-05-31 13:31:00.000000 xeus_python_shell-0.6.2/LICENSE
--rw-r--r--   0 martin    (1000) martin    (1000)       16 2024-05-31 13:31:00.000000 xeus_python_shell-0.6.2/MANIFEST.in
--rw-r--r--   0 martin    (1000) martin    (1000)      988 2024-05-31 13:32:23.579568 xeus_python_shell-0.6.2/PKG-INFO
--rw-r--r--   0 martin    (1000) martin    (1000)      101 2024-05-31 13:31:00.000000 xeus_python_shell-0.6.2/README.md
--rw-r--r--   0 martin    (1000) martin    (1000)       38 2024-05-31 13:32:23.579568 xeus_python_shell-0.6.2/setup.cfg
--rw-r--r--   0 martin    (1000) martin    (1000)     1144 2024-05-31 13:31:52.000000 xeus_python_shell-0.6.2/setup.py
-drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2024-05-31 13:32:23.578568 xeus_python_shell-0.6.2/xeus_python_shell/
--rw-r--r--   0 martin    (1000) martin    (1000)        0 2024-05-31 13:31:00.000000 xeus_python_shell-0.6.2/xeus_python_shell/__init__.py
--rw-r--r--   0 martin    (1000) martin    (1000)      587 2024-05-31 13:31:00.000000 xeus_python_shell-0.6.2/xeus_python_shell/compiler.py
--rw-r--r--   0 martin    (1000) martin    (1000)     3805 2024-05-31 13:31:00.000000 xeus_python_shell-0.6.2/xeus_python_shell/debugger.py
--rw-r--r--   0 martin    (1000) martin    (1000)     1383 2024-05-31 13:31:00.000000 xeus_python_shell-0.6.2/xeus_python_shell/display.py
--rw-r--r--   0 martin    (1000) martin    (1000)     3584 2024-05-31 13:31:01.000000 xeus_python_shell-0.6.2/xeus_python_shell/shell.py
-drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2024-05-31 13:32:23.578568 xeus_python_shell-0.6.2/xeus_python_shell.egg-info/
--rw-r--r--   0 martin    (1000) martin    (1000)      988 2024-05-31 13:32:23.000000 xeus_python_shell-0.6.2/xeus_python_shell.egg-info/PKG-INFO
--rw-r--r--   0 martin    (1000) martin    (1000)      388 2024-05-31 13:32:23.000000 xeus_python_shell-0.6.2/xeus_python_shell.egg-info/SOURCES.txt
--rw-r--r--   0 martin    (1000) martin    (1000)        1 2024-05-31 13:32:23.000000 xeus_python_shell-0.6.2/xeus_python_shell.egg-info/dependency_links.txt
--rw-r--r--   0 martin    (1000) martin    (1000)       73 2024-05-31 13:32:23.000000 xeus_python_shell-0.6.2/xeus_python_shell.egg-info/requires.txt
--rw-r--r--   0 martin    (1000) martin    (1000)       18 2024-05-31 13:32:23.000000 xeus_python_shell-0.6.2/xeus_python_shell.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:15:18.024384 xeus_python_shell-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-06-03 07:15:09.000000 xeus_python_shell-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-06-03 07:15:09.000000 xeus_python_shell-0.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-06-03 07:15:18.020384 xeus_python_shell-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-06-03 07:15:09.000000 xeus_python_shell-0.6.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 07:15:18.024384 xeus_python_shell-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-06-03 07:15:09.000000 xeus_python_shell-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:15:18.020384 xeus_python_shell-0.6.3/xeus_python_shell/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 07:15:09.000000 xeus_python_shell-0.6.3/xeus_python_shell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-06-03 07:15:09.000000 xeus_python_shell-0.6.3/xeus_python_shell/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-06-03 07:15:09.000000 xeus_python_shell-0.6.3/xeus_python_shell/debugger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-06-03 07:15:09.000000 xeus_python_shell-0.6.3/xeus_python_shell/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-06-03 07:15:09.000000 xeus_python_shell-0.6.3/xeus_python_shell/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:15:18.020384 xeus_python_shell-0.6.3/xeus_python_shell.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-06-03 07:15:18.000000 xeus_python_shell-0.6.3/xeus_python_shell.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-06-03 07:15:18.000000 xeus_python_shell-0.6.3/xeus_python_shell.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 07:15:18.000000 xeus_python_shell-0.6.3/xeus_python_shell.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-06-03 07:15:18.000000 xeus_python_shell-0.6.3/xeus_python_shell.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-06-03 07:15:18.000000 xeus_python_shell-0.6.3/xeus_python_shell.egg-info/top_level.txt
```

### Comparing `xeus_python_shell-0.6.2/LICENSE` & `xeus_python_shell-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xeus_python_shell-0.6.2/PKG-INFO` & `xeus_python_shell-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xeus-python-shell
-Version: 0.6.2
+Version: 0.6.3
 Summary: The xeus-python core python logic.
 Home-page: https://github.com/jupyter-xeus/xeus-python-shell
 Author: QuantStack dev team
 Maintainer: QuantStack dev team
 License: BSD 3-Clause
 Keywords: python ipython xeus-python
 Platform: any
```

### Comparing `xeus_python_shell-0.6.2/setup.py` & `xeus_python_shell-0.6.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup, find_packages
 
 __AUTHOR__ = 'QuantStack dev team'
 
 setup(
     name='xeus-python-shell',
-    version='0.6.2',
+    version='0.6.3',
     description='The xeus-python core python logic.',
     author=__AUTHOR__,
     maintainer=__AUTHOR__,
     url='https://github.com/jupyter-xeus/xeus-python-shell',
     license='BSD 3-Clause',
     keywords='python ipython xeus-python',
     packages=find_packages(exclude=['test']),
```

### Comparing `xeus_python_shell-0.6.2/xeus_python_shell/compiler.py` & `xeus_python_shell-0.6.3/xeus_python_shell/compiler.py`

 * *Files identical despite different names*

### Comparing `xeus_python_shell-0.6.2/xeus_python_shell/debugger.py` & `xeus_python_shell-0.6.3/xeus_python_shell/debugger.py`

 * *Files identical despite different names*

### Comparing `xeus_python_shell-0.6.2/xeus_python_shell/display.py` & `xeus_python_shell-0.6.3/xeus_python_shell/display.py`

 * *Files identical despite different names*

### Comparing `xeus_python_shell-0.6.2/xeus_python_shell/shell.py` & `xeus_python_shell-0.6.3/xeus_python_shell/shell.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     def __init__(self, shell=None, config=None, **traits):
         self.enabled = False
         super(LiteHistoryManager, self).__init__(shell=shell, config=config, **traits)
 
 
 class XPythonShell(InteractiveShell):
-    def __init__(self, use_jedi, *args, **kwargs):
+    def __init__(self, use_jedi=False, *args, **kwargs):
         super(XPythonShell, self).__init__(*args, **kwargs)
 
         self.kernel = None
         self.Completer.use_jedi = use_jedi
 
     def enable_gui(self, gui=None):
         """Not implemented yet."""
@@ -72,15 +72,15 @@
             cursor_end = cursor_pos
             matches = []
 
         return matches, cursor_start, cursor_end
 
 
 class XPythonShellApp(BaseIPythonApplication, InteractiveShellApp):
-    def initialize(self, use_jedi, argv=None):
+    def initialize(self, use_jedi=False, argv=None):
         super(XPythonShellApp, self).initialize(argv)
 
         self.user_ns = {}
 
         # self.init_io() ?
 
         self.init_path()
@@ -92,15 +92,15 @@
 
         self.init_extensions()
         self.init_code()
 
         sys.stdout.flush()
         sys.stderr.flush()
 
-    def init_shell(self, use_jedi):
+    def init_shell(self, use_jedi=False):
         self.shell = XPythonShell.instance(
             use_jedi,
             display_pub_class=XDisplayPublisher,
             displayhook_class=XDisplayHook,
             compiler_class=XCachingCompiler,
             user_ns=self.user_ns,
         )
```

### Comparing `xeus_python_shell-0.6.2/xeus_python_shell.egg-info/PKG-INFO` & `xeus_python_shell-0.6.3/xeus_python_shell.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xeus-python-shell
-Version: 0.6.2
+Version: 0.6.3
 Summary: The xeus-python core python logic.
 Home-page: https://github.com/jupyter-xeus/xeus-python-shell
 Author: QuantStack dev team
 Maintainer: QuantStack dev team
 License: BSD 3-Clause
 Keywords: python ipython xeus-python
 Platform: any
```

