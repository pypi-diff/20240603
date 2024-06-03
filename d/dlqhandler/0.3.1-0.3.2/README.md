# Comparing `tmp/dlqhandler-0.3.1.tar.gz` & `tmp/dlqhandler-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlqhandler-0.3.1.tar", last modified: Mon Jun  3 06:36:14 2024, max compression
+gzip compressed data, was "dlqhandler-0.3.2.tar", last modified: Mon Jun  3 06:45:04 2024, max compression
```

## Comparing `dlqhandler-0.3.1.tar` & `dlqhandler-0.3.2.tar`

### file list

```diff
@@ -1,22 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:36:14.094975 dlqhandler-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-06-03 06:35:45.000000 dlqhandler-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-06-03 06:36:14.094975 dlqhandler-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-06-03 06:35:45.000000 dlqhandler-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:36:14.094975 dlqhandler-0.3.1/dlqhandler/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-06-03 06:35:45.000000 dlqhandler-0.3.1/dlqhandler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:36:14.094975 dlqhandler-0.3.1/dlqhandler/dataprovider/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 06:35:45.000000 dlqhandler-0.3.1/dlqhandler/dataprovider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-06-03 06:35:45.000000 dlqhandler-0.3.1/dlqhandler/dataprovider/send_to_aws_sqs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-06-03 06:35:45.000000 dlqhandler-0.3.1/dlqhandler/dataprovider/sqs_queue.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:36:14.094975 dlqhandler-0.3.1/dlqhandler/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 06:35:45.000000 dlqhandler-0.3.1/dlqhandler/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-06-03 06:35:45.000000 dlqhandler-0.3.1/dlqhandler/services/cloudwatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-06-03 06:35:45.000000 dlqhandler-0.3.1/dlqhandler/services/process.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:36:14.094975 dlqhandler-0.3.1/dlqhandler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-06-03 06:36:13.000000 dlqhandler-0.3.1/dlqhandler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-06-03 06:36:14.000000 dlqhandler-0.3.1/dlqhandler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 06:36:13.000000 dlqhandler-0.3.1/dlqhandler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-06-03 06:36:13.000000 dlqhandler-0.3.1/dlqhandler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-06-03 06:36:13.000000 dlqhandler-0.3.1/dlqhandler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 06:36:14.094975 dlqhandler-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-06-03 06:35:45.000000 dlqhandler-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:45:04.532834 dlqhandler-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-06-03 06:44:42.000000 dlqhandler-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-06-03 06:45:04.532834 dlqhandler-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-06-03 06:44:42.000000 dlqhandler-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:45:04.528834 dlqhandler-0.3.2/dlqhandler/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-06-03 06:44:42.000000 dlqhandler-0.3.2/dlqhandler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:45:04.532834 dlqhandler-0.3.2/dlqhandler/dataprovider/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 06:44:42.000000 dlqhandler-0.3.2/dlqhandler/dataprovider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-06-03 06:44:42.000000 dlqhandler-0.3.2/dlqhandler/dataprovider/send_to_aws_sqs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-06-03 06:44:42.000000 dlqhandler-0.3.2/dlqhandler/dataprovider/sqs_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:45:04.532834 dlqhandler-0.3.2/dlqhandler/event/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-06-03 06:44:42.000000 dlqhandler-0.3.2/dlqhandler/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-06-03 06:44:42.000000 dlqhandler-0.3.2/dlqhandler/event/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:45:04.532834 dlqhandler-0.3.2/dlqhandler/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 06:44:42.000000 dlqhandler-0.3.2/dlqhandler/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-06-03 06:44:42.000000 dlqhandler-0.3.2/dlqhandler/services/cloudwatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-06-03 06:44:42.000000 dlqhandler-0.3.2/dlqhandler/services/process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:45:04.532834 dlqhandler-0.3.2/dlqhandler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-06-03 06:45:04.000000 dlqhandler-0.3.2/dlqhandler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-06-03 06:45:04.000000 dlqhandler-0.3.2/dlqhandler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 06:45:04.000000 dlqhandler-0.3.2/dlqhandler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-06-03 06:45:04.000000 dlqhandler-0.3.2/dlqhandler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-06-03 06:45:04.000000 dlqhandler-0.3.2/dlqhandler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 06:45:04.532834 dlqhandler-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-06-03 06:44:42.000000 dlqhandler-0.3.2/setup.py
```

### Comparing `dlqhandler-0.3.1/LICENSE` & `dlqhandler-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dlqhandler-0.3.1/PKG-INFO` & `dlqhandler-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlqhandler
-Version: 0.3.1
+Version: 0.3.2
 Summary: A library for handling DLQ messages in AWS SQS
 Home-page: https://github.com/seuusuario/dlq_handler_lib
 Author: Marcelo Ferreira
 Author-email: jaytilangus@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dlqhandler-0.3.1/README.md` & `dlqhandler-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `dlqhandler-0.3.1/dlqhandler/dataprovider/send_to_aws_sqs.py` & `dlqhandler-0.3.2/dlqhandler/dataprovider/send_to_aws_sqs.py`

 * *Files identical despite different names*

### Comparing `dlqhandler-0.3.1/dlqhandler/dataprovider/sqs_queue.py` & `dlqhandler-0.3.2/dlqhandler/dataprovider/sqs_queue.py`

 * *Files identical despite different names*

### Comparing `dlqhandler-0.3.1/dlqhandler/services/cloudwatch.py` & `dlqhandler-0.3.2/dlqhandler/services/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `dlqhandler-0.3.1/dlqhandler/services/process.py` & `dlqhandler-0.3.2/dlqhandler/services/process.py`

 * *Files identical despite different names*

### Comparing `dlqhandler-0.3.1/dlqhandler.egg-info/PKG-INFO` & `dlqhandler-0.3.2/dlqhandler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlqhandler
-Version: 0.3.1
+Version: 0.3.2
 Summary: A library for handling DLQ messages in AWS SQS
 Home-page: https://github.com/seuusuario/dlq_handler_lib
 Author: Marcelo Ferreira
 Author-email: jaytilangus@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dlqhandler-0.3.1/setup.py` & `dlqhandler-0.3.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='dlqhandler',
-    version="0.3.1",
-    packages=['dlqhandler', 'dlqhandler.services', 'dlqhandler.dataprovider'],
+    version="0.3.2",
+    packages=['dlqhandler', 'dlqhandler.services', 'dlqhandler.dataprovider', 'dlqhandler.event'],
     install_requires=[
         'boto3',
         'mock'
     ],
     author="Marcelo Ferreira",
     author_email="jaytilangus@gmail.com",
     description="A library for handling DLQ messages in AWS SQS",
```

