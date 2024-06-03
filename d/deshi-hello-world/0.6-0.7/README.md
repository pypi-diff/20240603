# Comparing `tmp/deshi_hello_world-0.6.tar.gz` & `tmp/deshi_hello_world-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deshi_hello_world-0.6.tar", last modified: Mon Jun  3 03:00:21 2024, max compression
+gzip compressed data, was "deshi_hello_world-0.7.tar", last modified: Mon Jun  3 03:03:43 2024, max compression
```

## Comparing `deshi_hello_world-0.6.tar` & `deshi_hello_world-0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 deshi     (1000) deshi     (1000)        0 2024-06-03 03:00:21.837399 deshi_hello_world-0.6/
--rw-r--r--   0 deshi     (1000) deshi     (1000)      208 2024-06-03 03:00:21.837399 deshi_hello_world-0.6/PKG-INFO
--rw-r--r--   0 deshi     (1000) deshi     (1000)       33 2024-06-02 18:42:56.000000 deshi_hello_world-0.6/README.md
-drwxr-xr-x   0 deshi     (1000) deshi     (1000)        0 2024-06-03 03:00:21.837399 deshi_hello_world-0.6/deshi_hello_world/
--rw-r--r--   0 deshi     (1000) deshi     (1000)      138 2024-06-03 02:59:49.000000 deshi_hello_world-0.6/deshi_hello_world/__init__.py
--rw-r--r--   0 deshi     (1000) deshi     (1000)      553 2024-06-03 02:59:51.000000 deshi_hello_world-0.6/deshi_hello_world/cli.py
-drwxr-xr-x   0 deshi     (1000) deshi     (1000)        0 2024-06-03 03:00:21.837399 deshi_hello_world-0.6/deshi_hello_world.egg-info/
--rw-r--r--   0 deshi     (1000) deshi     (1000)      208 2024-06-03 03:00:21.000000 deshi_hello_world-0.6/deshi_hello_world.egg-info/PKG-INFO
--rw-r--r--   0 deshi     (1000) deshi     (1000)      357 2024-06-03 03:00:21.000000 deshi_hello_world-0.6/deshi_hello_world.egg-info/SOURCES.txt
--rw-r--r--   0 deshi     (1000) deshi     (1000)        1 2024-06-03 03:00:21.000000 deshi_hello_world-0.6/deshi_hello_world.egg-info/dependency_links.txt
--rw-r--r--   0 deshi     (1000) deshi     (1000)      104 2024-06-03 03:00:21.000000 deshi_hello_world-0.6/deshi_hello_world.egg-info/entry_points.txt
--rw-r--r--   0 deshi     (1000) deshi     (1000)        6 2024-06-03 03:00:21.000000 deshi_hello_world-0.6/deshi_hello_world.egg-info/requires.txt
--rw-r--r--   0 deshi     (1000) deshi     (1000)       18 2024-06-03 03:00:21.000000 deshi_hello_world-0.6/deshi_hello_world.egg-info/top_level.txt
--rw-r--r--   0 deshi     (1000) deshi     (1000)       79 2024-06-03 03:00:21.837399 deshi_hello_world-0.6/setup.cfg
--rw-r--r--   0 deshi     (1000) deshi     (1000)      519 2024-06-03 03:00:04.000000 deshi_hello_world-0.6/setup.py
-drwxr-xr-x   0 deshi     (1000) deshi     (1000)        0 2024-06-03 03:00:21.837399 deshi_hello_world-0.6/tests/
--rw-r--r--   0 deshi     (1000) deshi     (1000)      153 2024-06-03 02:39:21.000000 deshi_hello_world-0.6/tests/test_hello_world.py
+drwxr-xr-x   0 deshi     (1000) deshi     (1000)        0 2024-06-03 03:03:43.037346 deshi_hello_world-0.7/
+-rw-r--r--   0 deshi     (1000) deshi     (1000)      208 2024-06-03 03:03:43.037346 deshi_hello_world-0.7/PKG-INFO
+-rw-r--r--   0 deshi     (1000) deshi     (1000)       33 2024-06-02 18:42:56.000000 deshi_hello_world-0.7/README.md
+drwxr-xr-x   0 deshi     (1000) deshi     (1000)        0 2024-06-03 03:03:43.037346 deshi_hello_world-0.7/deshi_hello_world/
+-rw-r--r--   0 deshi     (1000) deshi     (1000)      138 2024-06-03 03:03:20.000000 deshi_hello_world-0.7/deshi_hello_world/__init__.py
+-rw-r--r--   0 deshi     (1000) deshi     (1000)      559 2024-06-03 03:03:16.000000 deshi_hello_world-0.7/deshi_hello_world/cli.py
+drwxr-xr-x   0 deshi     (1000) deshi     (1000)        0 2024-06-03 03:03:43.037346 deshi_hello_world-0.7/deshi_hello_world.egg-info/
+-rw-r--r--   0 deshi     (1000) deshi     (1000)      208 2024-06-03 03:03:42.000000 deshi_hello_world-0.7/deshi_hello_world.egg-info/PKG-INFO
+-rw-r--r--   0 deshi     (1000) deshi     (1000)      357 2024-06-03 03:03:43.000000 deshi_hello_world-0.7/deshi_hello_world.egg-info/SOURCES.txt
+-rw-r--r--   0 deshi     (1000) deshi     (1000)        1 2024-06-03 03:03:42.000000 deshi_hello_world-0.7/deshi_hello_world.egg-info/dependency_links.txt
+-rw-r--r--   0 deshi     (1000) deshi     (1000)      116 2024-06-03 03:03:43.000000 deshi_hello_world-0.7/deshi_hello_world.egg-info/entry_points.txt
+-rw-r--r--   0 deshi     (1000) deshi     (1000)        6 2024-06-03 03:03:43.000000 deshi_hello_world-0.7/deshi_hello_world.egg-info/requires.txt
+-rw-r--r--   0 deshi     (1000) deshi     (1000)       18 2024-06-03 03:03:43.000000 deshi_hello_world-0.7/deshi_hello_world.egg-info/top_level.txt
+-rw-r--r--   0 deshi     (1000) deshi     (1000)       79 2024-06-03 03:03:43.037346 deshi_hello_world-0.7/setup.cfg
+-rw-r--r--   0 deshi     (1000) deshi     (1000)      531 2024-06-03 03:03:37.000000 deshi_hello_world-0.7/setup.py
+drwxr-xr-x   0 deshi     (1000) deshi     (1000)        0 2024-06-03 03:03:43.037346 deshi_hello_world-0.7/tests/
+-rw-r--r--   0 deshi     (1000) deshi     (1000)      153 2024-06-03 02:39:21.000000 deshi_hello_world-0.7/tests/test_hello_world.py
```

### Comparing `deshi_hello_world-0.6/deshi_hello_world/cli.py` & `deshi_hello_world-0.7/deshi_hello_world/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # hello_world/cli.py
 
 import click
-from hello_world import hello, multiply
+from deshi_hello_world import hello, multiply
 
 @click.command()
 def greet():
     """Simple program that greets the user."""
     click.echo(hello())
 
 @click.command()
```

### Comparing `deshi_hello_world-0.6/setup.py` & `deshi_hello_world-0.7/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # setup.py
 from setuptools import setup, find_packages
 
 setup(
     name='deshi_hello_world',
-    version='0.6',
+    version='0.7',
     description='A simple hello world package with multiplication functionality',
     author='deshi',
     author_email='deshithabollina28@gmail.com',
     packages=find_packages(),
     install_requires=[
         'click',
     ],
     entry_points={
         'console_scripts': [
-            'deshi-greet=hello_world.cli:greet',
-            'deshi-multiply=hello_world.cli:multiply_command',
+            'deshi-greet=deshi_hello_world.cli:greet',
+            'deshi-multiply=deshi_hello_world.cli:multiply_command',
         ],
     },
 )
```

