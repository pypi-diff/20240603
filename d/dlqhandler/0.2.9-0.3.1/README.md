# Comparing `tmp/dlqhandler-0.2.9.tar.gz` & `tmp/dlqhandler-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlqhandler-0.2.9.tar", last modified: Fri May 31 16:42:43 2024, max compression
+gzip compressed data, was "dlqhandler-0.3.1.tar", last modified: Mon Jun  3 06:36:14 2024, max compression
```

## Comparing `dlqhandler-0.2.9.tar` & `dlqhandler-0.3.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:42:43.701275 dlqhandler-0.2.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-31 16:42:25.000000 dlqhandler-0.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-31 16:42:43.701275 dlqhandler-0.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-31 16:42:25.000000 dlqhandler-0.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:42:43.701275 dlqhandler-0.2.9/dlqhandler/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-31 16:42:25.000000 dlqhandler-0.2.9/dlqhandler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:42:43.701275 dlqhandler-0.2.9/dlqhandler/dataprovider/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 16:42:25.000000 dlqhandler-0.2.9/dlqhandler/dataprovider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-31 16:42:25.000000 dlqhandler-0.2.9/dlqhandler/dataprovider/send_to_aws_sqs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-31 16:42:25.000000 dlqhandler-0.2.9/dlqhandler/dataprovider/sqs_queue.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:42:43.701275 dlqhandler-0.2.9/dlqhandler/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 16:42:25.000000 dlqhandler-0.2.9/dlqhandler/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-31 16:42:25.000000 dlqhandler-0.2.9/dlqhandler/services/cloudwatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-05-31 16:42:25.000000 dlqhandler-0.2.9/dlqhandler/services/process.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:42:43.701275 dlqhandler-0.2.9/dlqhandler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-31 16:42:43.000000 dlqhandler-0.2.9/dlqhandler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-31 16:42:43.000000 dlqhandler-0.2.9/dlqhandler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 16:42:43.000000 dlqhandler-0.2.9/dlqhandler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-31 16:42:43.000000 dlqhandler-0.2.9/dlqhandler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-31 16:42:43.000000 dlqhandler-0.2.9/dlqhandler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 16:42:43.701275 dlqhandler-0.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-31 16:42:25.000000 dlqhandler-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:36:14.094975 dlqhandler-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-06-03 06:35:45.000000 dlqhandler-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-06-03 06:36:14.094975 dlqhandler-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-06-03 06:35:45.000000 dlqhandler-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:36:14.094975 dlqhandler-0.3.1/dlqhandler/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-06-03 06:35:45.000000 dlqhandler-0.3.1/dlqhandler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:36:14.094975 dlqhandler-0.3.1/dlqhandler/dataprovider/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 06:35:45.000000 dlqhandler-0.3.1/dlqhandler/dataprovider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-06-03 06:35:45.000000 dlqhandler-0.3.1/dlqhandler/dataprovider/send_to_aws_sqs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-06-03 06:35:45.000000 dlqhandler-0.3.1/dlqhandler/dataprovider/sqs_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:36:14.094975 dlqhandler-0.3.1/dlqhandler/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 06:35:45.000000 dlqhandler-0.3.1/dlqhandler/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-06-03 06:35:45.000000 dlqhandler-0.3.1/dlqhandler/services/cloudwatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-06-03 06:35:45.000000 dlqhandler-0.3.1/dlqhandler/services/process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 06:36:14.094975 dlqhandler-0.3.1/dlqhandler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-06-03 06:36:13.000000 dlqhandler-0.3.1/dlqhandler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-06-03 06:36:14.000000 dlqhandler-0.3.1/dlqhandler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 06:36:13.000000 dlqhandler-0.3.1/dlqhandler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-06-03 06:36:13.000000 dlqhandler-0.3.1/dlqhandler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-06-03 06:36:13.000000 dlqhandler-0.3.1/dlqhandler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 06:36:14.094975 dlqhandler-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-06-03 06:35:45.000000 dlqhandler-0.3.1/setup.py
```

### Comparing `dlqhandler-0.2.9/LICENSE` & `dlqhandler-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dlqhandler-0.2.9/PKG-INFO` & `dlqhandler-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlqhandler
-Version: 0.2.9
+Version: 0.3.1
 Summary: A library for handling DLQ messages in AWS SQS
 Home-page: https://github.com/seuusuario/dlq_handler_lib
 Author: Marcelo Ferreira
 Author-email: jaytilangus@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dlqhandler-0.2.9/README.md` & `dlqhandler-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `dlqhandler-0.2.9/dlqhandler/dataprovider/send_to_aws_sqs.py` & `dlqhandler-0.3.1/dlqhandler/dataprovider/send_to_aws_sqs.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,16 @@
     def __init__(self, env):
         self.env = env
 
     def send_message_to_queue(self, messagebody):
         try:
             logger.info("enviar_mensagem_sqs >> %s", json.loads(messagebody))
             sqs_link = self.env.url_sqs_orquestrador()
-            sqs = boto3.client(service_name="sqs")
+            session = boto3.Session()
+            sqs = session.client(service_name="sqs")
 
             if self.env != "TAAC":
                 sqs.send_message(
                     QueueUrl=sqs_link,
                     MessageBody=messagebody
                 )
```

### Comparing `dlqhandler-0.2.9/dlqhandler/services/cloudwatch.py` & `dlqhandler-0.3.1/dlqhandler/services/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `dlqhandler-0.2.9/dlqhandler/services/process.py` & `dlqhandler-0.3.1/dlqhandler/services/process.py`

 * *Files identical despite different names*

### Comparing `dlqhandler-0.2.9/dlqhandler.egg-info/PKG-INFO` & `dlqhandler-0.3.1/dlqhandler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlqhandler
-Version: 0.2.9
+Version: 0.3.1
 Summary: A library for handling DLQ messages in AWS SQS
 Home-page: https://github.com/seuusuario/dlq_handler_lib
 Author: Marcelo Ferreira
 Author-email: jaytilangus@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dlqhandler-0.2.9/setup.py` & `dlqhandler-0.3.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='dlqhandler',
-    version="0.2.9",
+    version="0.3.1",
     packages=['dlqhandler', 'dlqhandler.services', 'dlqhandler.dataprovider'],
     install_requires=[
         'boto3',
         'mock'
     ],
     author="Marcelo Ferreira",
     author_email="jaytilangus@gmail.com",
```

