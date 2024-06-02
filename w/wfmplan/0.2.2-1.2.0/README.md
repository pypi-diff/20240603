# Comparing `tmp/wfmplan-0.2.2.tar.gz` & `tmp/wfmplan-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wfmplan-0.2.2.tar", last modified: Sun Jun  2 16:15:58 2024, max compression
+gzip compressed data, was "wfmplan-1.2.0.tar", last modified: Sun Jun  2 16:57:13 2024, max compression
```

## Comparing `wfmplan-0.2.2.tar` & `wfmplan-1.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:15:58.956600 wfmplan-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-06-02 16:15:48.000000 wfmplan-0.2.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-06-02 16:15:58.956600 wfmplan-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-06-02 16:15:48.000000 wfmplan-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 16:15:58.956600 wfmplan-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-06-02 16:15:48.000000 wfmplan-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:15:58.952600 wfmplan-0.2.2/wfmplan/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:15:58.952600 wfmplan-0.2.2/wfmplan/AgentOptimizer/
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-06-02 16:15:48.000000 wfmplan-0.2.2/wfmplan/AgentOptimizer/BatchOptimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5845 2024-06-02 16:15:48.000000 wfmplan-0.2.2/wfmplan/AgentOptimizer/Optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-06-02 16:15:48.000000 wfmplan-0.2.2/wfmplan/AgentOptimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-06-02 16:15:48.000000 wfmplan-0.2.2/wfmplan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:15:58.956600 wfmplan-0.2.2/wfmplan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-06-02 16:15:58.000000 wfmplan-0.2.2/wfmplan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-06-02 16:15:58.000000 wfmplan-0.2.2/wfmplan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 16:15:58.000000 wfmplan-0.2.2/wfmplan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-02 16:15:58.000000 wfmplan-0.2.2/wfmplan.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-06-02 16:15:58.000000 wfmplan-0.2.2/wfmplan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-06-02 16:15:58.000000 wfmplan-0.2.2/wfmplan.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:57:13.284753 wfmplan-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-06-02 16:57:09.000000 wfmplan-1.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-06-02 16:57:13.280753 wfmplan-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-06-02 16:57:09.000000 wfmplan-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 16:57:13.284753 wfmplan-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-06-02 16:57:09.000000 wfmplan-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:57:13.280753 wfmplan-1.2.0/wfmplan/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:57:13.280753 wfmplan-1.2.0/wfmplan/AgentOptimizer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-06-02 16:57:09.000000 wfmplan-1.2.0/wfmplan/AgentOptimizer/BatchOptimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5845 2024-06-02 16:57:09.000000 wfmplan-1.2.0/wfmplan/AgentOptimizer/Optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-06-02 16:57:09.000000 wfmplan-1.2.0/wfmplan/AgentOptimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-06-02 16:57:09.000000 wfmplan-1.2.0/wfmplan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:57:13.280753 wfmplan-1.2.0/wfmplan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-06-02 16:57:13.000000 wfmplan-1.2.0/wfmplan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-06-02 16:57:13.000000 wfmplan-1.2.0/wfmplan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 16:57:13.000000 wfmplan-1.2.0/wfmplan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-02 16:57:13.000000 wfmplan-1.2.0/wfmplan.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-06-02 16:57:13.000000 wfmplan-1.2.0/wfmplan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-06-02 16:57:13.000000 wfmplan-1.2.0/wfmplan.egg-info/top_level.txt
```

### Comparing `wfmplan-0.2.2/LICENSE.txt` & `wfmplan-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wfmplan-0.2.2/setup.py` & `wfmplan-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="wfmplan",
-    version="0.2.2",
+    version="1.2.0",
     description="Optimization library for workforce management planning",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/laddha-rishi/wfmplan",
     author="Rishi Laddha",
     author_email="laddha.rishi@gmail.com",
     license="MIT",
@@ -34,8 +34,8 @@
     keywords="workforce management optimization",
     python_requires='>=3.8',
     entry_points={
         'console_scripts': [
             'wfmplan=wfmplan:main',
         ],
     },
-)
+)
```

### Comparing `wfmplan-0.2.2/wfmplan/AgentOptimizer/Optimizer.py` & `wfmplan-1.2.0/wfmplan/AgentOptimizer/Optimizer.py`

 * *Files identical despite different names*

