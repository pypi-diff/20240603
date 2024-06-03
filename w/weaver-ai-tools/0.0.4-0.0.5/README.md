# Comparing `tmp/weaver-ai-tools-0.0.4.tar.gz` & `tmp/weaver-ai-tools-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weaver-ai-tools-0.0.4.tar", last modified: Mon Jun  3 15:18:46 2024, max compression
+gzip compressed data, was "weaver-ai-tools-0.0.5.tar", last modified: Mon Jun  3 15:24:11 2024, max compression
```

## Comparing `weaver-ai-tools-0.0.4.tar` & `weaver-ai-tools-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 artemmeahkov   (501) staff       (20)        0 2024-06-03 15:18:46.153319 weaver-ai-tools-0.0.4/
--rw-r--r--   0 artemmeahkov   (501) staff       (20)       59 2024-06-03 15:18:46.153209 weaver-ai-tools-0.0.4/PKG-INFO
--rw-r--r--   0 artemmeahkov   (501) staff       (20)       38 2024-06-03 15:18:46.153357 weaver-ai-tools-0.0.4/setup.cfg
--rw-r--r--   0 artemmeahkov   (501) staff       (20)      158 2024-06-02 14:08:12.000000 weaver-ai-tools-0.0.4/setup.py
-drwxr-xr-x   0 artemmeahkov   (501) staff       (20)        0 2024-06-03 15:18:46.152047 weaver-ai-tools-0.0.4/weaver_ai_tools/
--rw-r--r--   0 artemmeahkov   (501) staff       (20)        0 2024-05-26 07:19:50.000000 weaver-ai-tools-0.0.4/weaver_ai_tools/__init__.py
-drwxr-xr-x   0 artemmeahkov   (501) staff       (20)        0 2024-06-03 15:18:46.152932 weaver-ai-tools-0.0.4/weaver_ai_tools/v1/
--rw-r--r--   0 artemmeahkov   (501) staff       (20)        0 2024-05-27 07:15:04.000000 weaver-ai-tools-0.0.4/weaver_ai_tools/v1/__init__.py
--rw-r--r--   0 artemmeahkov   (501) staff       (20)     2954 2024-05-26 11:12:28.000000 weaver-ai-tools-0.0.4/weaver_ai_tools/v1/config.py
--rw-r--r--   0 artemmeahkov   (501) staff       (20)      589 2024-06-03 15:10:09.000000 weaver-ai-tools-0.0.4/weaver_ai_tools/v1/functions.py
-drwxr-xr-x   0 artemmeahkov   (501) staff       (20)        0 2024-06-03 15:18:46.152447 weaver-ai-tools-0.0.4/weaver_ai_tools.egg-info/
--rw-r--r--   0 artemmeahkov   (501) staff       (20)       59 2024-06-03 15:18:46.000000 weaver-ai-tools-0.0.4/weaver_ai_tools.egg-info/PKG-INFO
--rw-r--r--   0 artemmeahkov   (501) staff       (20)      284 2024-06-03 15:18:46.000000 weaver-ai-tools-0.0.4/weaver_ai_tools.egg-info/SOURCES.txt
--rw-r--r--   0 artemmeahkov   (501) staff       (20)        1 2024-06-03 15:18:46.000000 weaver-ai-tools-0.0.4/weaver_ai_tools.egg-info/dependency_links.txt
--rw-r--r--   0 artemmeahkov   (501) staff       (20)       16 2024-06-03 15:18:46.000000 weaver-ai-tools-0.0.4/weaver_ai_tools.egg-info/top_level.txt
+drwxr-xr-x   0 artemmeahkov   (501) staff       (20)        0 2024-06-03 15:24:11.379253 weaver-ai-tools-0.0.5/
+-rw-r--r--   0 artemmeahkov   (501) staff       (20)       59 2024-06-03 15:24:11.379138 weaver-ai-tools-0.0.5/PKG-INFO
+-rw-r--r--   0 artemmeahkov   (501) staff       (20)       38 2024-06-03 15:24:11.379291 weaver-ai-tools-0.0.5/setup.cfg
+-rw-r--r--   0 artemmeahkov   (501) staff       (20)      158 2024-06-03 15:23:24.000000 weaver-ai-tools-0.0.5/setup.py
+drwxr-xr-x   0 artemmeahkov   (501) staff       (20)        0 2024-06-03 15:24:11.378185 weaver-ai-tools-0.0.5/weaver_ai_tools/
+-rw-r--r--   0 artemmeahkov   (501) staff       (20)        0 2024-05-26 07:19:50.000000 weaver-ai-tools-0.0.5/weaver_ai_tools/__init__.py
+drwxr-xr-x   0 artemmeahkov   (501) staff       (20)        0 2024-06-03 15:24:11.378979 weaver-ai-tools-0.0.5/weaver_ai_tools/v1/
+-rw-r--r--   0 artemmeahkov   (501) staff       (20)        0 2024-05-27 07:15:04.000000 weaver-ai-tools-0.0.5/weaver_ai_tools/v1/__init__.py
+-rw-r--r--   0 artemmeahkov   (501) staff       (20)     2954 2024-05-26 11:12:28.000000 weaver-ai-tools-0.0.5/weaver_ai_tools/v1/config.py
+-rw-r--r--   0 artemmeahkov   (501) staff       (20)      589 2024-06-03 15:10:09.000000 weaver-ai-tools-0.0.5/weaver_ai_tools/v1/functions.py
+drwxr-xr-x   0 artemmeahkov   (501) staff       (20)        0 2024-06-03 15:24:11.378675 weaver-ai-tools-0.0.5/weaver_ai_tools.egg-info/
+-rw-r--r--   0 artemmeahkov   (501) staff       (20)       59 2024-06-03 15:24:11.000000 weaver-ai-tools-0.0.5/weaver_ai_tools.egg-info/PKG-INFO
+-rw-r--r--   0 artemmeahkov   (501) staff       (20)      284 2024-06-03 15:24:11.000000 weaver-ai-tools-0.0.5/weaver_ai_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 artemmeahkov   (501) staff       (20)        1 2024-06-03 15:24:11.000000 weaver-ai-tools-0.0.5/weaver_ai_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 artemmeahkov   (501) staff       (20)       16 2024-06-03 15:24:11.000000 weaver-ai-tools-0.0.5/weaver_ai_tools.egg-info/top_level.txt
```

### Comparing `weaver-ai-tools-0.0.4/weaver_ai_tools/v1/config.py` & `weaver-ai-tools-0.0.5/weaver_ai_tools/v1/config.py`

 * *Files identical despite different names*

### Comparing `weaver-ai-tools-0.0.4/weaver_ai_tools/v1/functions.py` & `weaver-ai-tools-0.0.5/weaver_ai_tools/v1/functions.py`

 * *Files identical despite different names*

