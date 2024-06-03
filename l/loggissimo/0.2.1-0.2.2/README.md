# Comparing `tmp/loggissimo-0.2.1.tar.gz` & `tmp/loggissimo-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loggissimo-0.2.1.tar", last modified: Fri May 31 11:15:18 2024, max compression
+gzip compressed data, was "loggissimo-0.2.2.tar", last modified: Mon Jun  3 03:47:21 2024, max compression
```

## Comparing `loggissimo-0.2.1.tar` & `loggissimo-0.2.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 11:15:18.055487 loggissimo-0.2.1/
--rw-r--r--   0 root         (0) root         (0)     1853 2024-05-31 11:15:18.055487 loggissimo-0.2.1/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)       12 2024-03-05 09:15:45.000000 loggissimo-0.2.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 11:15:18.055487 loggissimo-0.2.1/loggissimo/
--rw-rw-r--   0 root         (0) root         (0)       77 2024-05-31 11:15:17.000000 loggissimo-0.2.1/loggissimo/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    10210 2024-05-31 11:13:36.000000 loggissimo-0.2.1/loggissimo/_logger.py
--rwxrwxr-x   0 root         (0) root         (0)     3389 2024-05-31 11:12:34.000000 loggissimo-0.2.1/loggissimo/_style.py
--rw-rw-r--   0 root         (0) root         (0)     1496 2024-05-27 06:31:36.000000 loggissimo-0.2.1/loggissimo/_utils.py
--rw-rw-r--   0 root         (0) root         (0)      394 2024-05-31 03:53:19.000000 loggissimo-0.2.1/loggissimo/constants.py
--rw-rw-r--   0 root         (0) root         (0)      385 2024-05-27 06:31:48.000000 loggissimo-0.2.1/loggissimo/exceptions.py
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-15 10:35:22.000000 loggissimo-0.2.1/loggissimo/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 11:15:18.055487 loggissimo-0.2.1/loggissimo.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1853 2024-05-31 11:15:18.000000 loggissimo-0.2.1/loggissimo.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      353 2024-05-31 11:15:18.000000 loggissimo-0.2.1/loggissimo.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-31 11:15:18.000000 loggissimo-0.2.1/loggissimo.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-05-31 11:15:18.000000 loggissimo-0.2.1/loggissimo.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-05-31 11:15:18.000000 loggissimo-0.2.1/loggissimo.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)       63 2024-05-31 11:15:18.055487 loggissimo-0.2.1/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      730 2024-05-31 10:02:27.000000 loggissimo-0.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 03:47:21.651602 loggissimo-0.2.2/
+-rw-rw-r--   0 root         (0) root         (0)     1072 2024-05-31 10:08:00.000000 loggissimo-0.2.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1914 2024-06-03 03:47:21.651602 loggissimo-0.2.2/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     1563 2024-06-03 03:43:53.000000 loggissimo-0.2.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 03:47:21.651602 loggissimo-0.2.2/loggissimo/
+-rw-rw-r--   0 root         (0) root         (0)       77 2024-06-03 03:47:21.000000 loggissimo-0.2.2/loggissimo/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    10287 2024-06-03 03:45:50.000000 loggissimo-0.2.2/loggissimo/_logger.py
+-rwxrwxr-x   0 root         (0) root         (0)     3240 2024-05-31 11:24:15.000000 loggissimo-0.2.2/loggissimo/_style.py
+-rw-rw-r--   0 root         (0) root         (0)     1496 2024-05-27 06:31:36.000000 loggissimo-0.2.2/loggissimo/_utils.py
+-rw-rw-r--   0 root         (0) root         (0)      394 2024-05-31 03:53:19.000000 loggissimo-0.2.2/loggissimo/constants.py
+-rw-rw-r--   0 root         (0) root         (0)      385 2024-05-27 06:31:48.000000 loggissimo-0.2.2/loggissimo/exceptions.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-05-15 10:35:22.000000 loggissimo-0.2.2/loggissimo/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 03:47:21.651602 loggissimo-0.2.2/loggissimo.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1914 2024-06-03 03:47:21.000000 loggissimo-0.2.2/loggissimo.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      361 2024-06-03 03:47:21.000000 loggissimo-0.2.2/loggissimo.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-03 03:47:21.000000 loggissimo-0.2.2/loggissimo.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-06-03 03:47:21.000000 loggissimo-0.2.2/loggissimo.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-06-03 03:47:21.000000 loggissimo-0.2.2/loggissimo.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)       63 2024-06-03 03:47:21.651602 loggissimo-0.2.2/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      762 2024-06-03 03:46:58.000000 loggissimo-0.2.2/setup.py
```

### Comparing `loggissimo-0.2.1/PKG-INFO` & `loggissimo-0.2.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: loggissimo
-Version: 0.2.1
+Version: 0.2.2
 Summary: Awesome and simple logger
 Home-page: https://github.com/Sw1mmeR/loggissimo/tree/main
 Author: MikleSedrakyan & AfanasevAndrey
+Author-email: scriptdefender@yandex.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 ![Logo](https://github.com/Sw1mmeR/loggissimo/blob/main/assets/logo.png)
 
 # loggissimo
 
 Awesome and simple logger!
```

### Comparing `loggissimo-0.2.1/loggissimo/_logger.py` & `loggissimo-0.2.2/loggissimo/_logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,20 +103,23 @@
     def _log(self, level: Level, message: str):
         def colorize(do_not_colorize: bool):
             if do_not_colorize:
                 msg_t = self._format
             else:
                 msg_t = style(self._format, level)
 
-            return Template(msg_t).safe_substitute(
-                name=f"{name:30}",
-                time=f"{time}",
-                level=f"{level.name:<8}",
-                stack=f"{stack}",
-                text=f"{message}\n",
+            return (
+                Template(msg_t).safe_substitute(
+                    name=f"{name:30}",
+                    time=f"{time}",
+                    level=f"{level.name:<8}",
+                    stack=f"{stack}",
+                    text=f"{message}",
+                )
+                + "\n"
             )
 
         self.in_thread = self._check_threading()
         time_now = datetime.now()
         frame = sys._getframe(3)
 
         try:
```

### Comparing `loggissimo-0.2.1/loggissimo/_style.py` & `loggissimo-0.2.2/loggissimo/_style.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,19 +51,14 @@
             style=FontStyle.bold,
         ),
     }
 
     for style, value in style_format:
         format = format.replace(style, "")
         tag = Tag(style, value)
-        print(do_not_colorize)
-        if do_not_colorize:
-            styled[value[1:]] = tag.text
-            print(tag.text)
-            continue
         styled[value[1:]] = tag.colorized
 
     return Template(format).safe_substitute(**styled)
 
 
 class Tag:
     def __init__(self, tag: str, text: str, *args, **kwargs) -> None:
```

### Comparing `loggissimo-0.2.1/loggissimo/_utils.py` & `loggissimo-0.2.2/loggissimo/_utils.py`

 * *Files identical despite different names*

### Comparing `loggissimo-0.2.1/loggissimo.egg-info/PKG-INFO` & `loggissimo-0.2.2/loggissimo.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: loggissimo
-Version: 0.2.1
+Version: 0.2.2
 Summary: Awesome and simple logger
 Home-page: https://github.com/Sw1mmeR/loggissimo/tree/main
 Author: MikleSedrakyan & AfanasevAndrey
+Author-email: scriptdefender@yandex.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 ![Logo](https://github.com/Sw1mmeR/loggissimo/blob/main/assets/logo.png)
 
 # loggissimo
 
 Awesome and simple logger!
```

### Comparing `loggissimo-0.2.1/setup.py` & `loggissimo-0.2.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import loggissimo
 from setuptools import setup, find_packages
 
-with open("/home/sw1mmer/projects/loggissimo/loggissimo/README.md") as file:
+with open("README.md") as file:
     long_description = file.read()
 
 setup(
     name=loggissimo.__name__,
     version=loggissimo.__version__,
     author="MikleSedrakyan & AfanasevAndrey",
+    author_email="scriptdefender@yandex.ru",
     description="Awesome and simple logger",
+    license_files=("LICENSE",),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Sw1mmeR/loggissimo/tree/main",
     packages=find_packages(),
     package_data={
         loggissimo.__name__: ["py.typed"],
     },
```

