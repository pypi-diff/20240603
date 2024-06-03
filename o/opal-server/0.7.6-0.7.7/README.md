# Comparing `tmp/opal_server-0.7.6.tar.gz` & `tmp/opal-server-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opal_server-0.7.6.tar", last modified: Tue Apr 30 17:18:49 2024, max compression
+gzip compressed data, was "opal-server-0.7.7.tar", last modified: Mon Jun  3 13:38:17 2024, max compression
```

## Comparing `opal_server-0.7.6.tar` & `opal-server-0.7.7.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:49.207912 opal_server-0.7.6/
--rw-r--r--   0 roekatz    (501) staff       (20)    10196 2024-04-30 17:18:49.207451 opal_server-0.7.6/PKG-INFO
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:49.202300 opal_server-0.7.6/opal_server/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal_server-0.7.6/opal_server/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     2136 2023-05-29 10:10:14.000000 opal_server-0.7.6/opal_server/cli.py
--rw-r--r--   0 roekatz    (501) staff       (20)    11336 2024-04-30 12:59:10.000000 opal_server-0.7.6/opal_server/config.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:49.203740 opal_server-0.7.6/opal_server/data/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal_server-0.7.6/opal_server/data/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     5303 2023-06-20 17:01:29.000000 opal_server-0.7.6/opal_server/data/api.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4004 2024-04-30 13:01:51.000000 opal_server-0.7.6/opal_server/data/data_update_publisher.py
--rw-r--r--   0 roekatz    (501) staff       (20)    15201 2024-03-19 14:53:02.000000 opal_server-0.7.6/opal_server/git_fetcher.py
--rw-r--r--   0 roekatz    (501) staff       (20)      987 2022-12-08 13:40:17.000000 opal_server-0.7.6/opal_server/loadlimiting.py
--rw-r--r--   0 roekatz    (501) staff       (20)      153 2022-12-08 13:40:17.000000 opal_server-0.7.6/opal_server/main.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:49.203872 opal_server-0.7.6/opal_server/policy/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal_server-0.7.6/opal_server/policy/__init__.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:49.204103 opal_server-0.7.6/opal_server/policy/bundles/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal_server-0.7.6/opal_server/policy/bundles/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4447 2023-05-29 10:10:14.000000 opal_server-0.7.6/opal_server/policy/bundles/api.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:49.204701 opal_server-0.7.6/opal_server/policy/watcher/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2023-05-29 10:10:14.000000 opal_server-0.7.6/opal_server/policy/watcher/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4529 2023-06-20 17:01:29.000000 opal_server-0.7.6/opal_server/policy/watcher/callbacks.py
--rw-r--r--   0 roekatz    (501) staff       (20)     6662 2024-04-30 12:59:10.000000 opal_server-0.7.6/opal_server/policy/watcher/factory.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4767 2023-06-27 11:27:39.000000 opal_server-0.7.6/opal_server/policy/watcher/task.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:49.205297 opal_server-0.7.6/opal_server/policy/webhook/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal_server-0.7.6/opal_server/policy/webhook/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     5690 2024-03-19 14:53:02.000000 opal_server-0.7.6/opal_server/policy/webhook/api.py
--rw-r--r--   0 roekatz    (501) staff       (20)     6110 2023-05-29 10:10:14.000000 opal_server-0.7.6/opal_server/policy/webhook/deps.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1234 2022-12-08 13:40:17.000000 opal_server-0.7.6/opal_server/policy/webhook/listener.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1331 2022-12-08 13:40:17.000000 opal_server-0.7.6/opal_server/publisher.py
--rw-r--r--   0 roekatz    (501) staff       (20)     8009 2024-03-19 14:53:02.000000 opal_server-0.7.6/opal_server/pubsub.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1404 2023-10-04 11:07:26.000000 opal_server-0.7.6/opal_server/redis.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:49.206198 opal_server-0.7.6/opal_server/scopes/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal_server-0.7.6/opal_server/scopes/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)    12784 2024-03-19 14:53:02.000000 opal_server-0.7.6/opal_server/scopes/api.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1621 2023-05-29 10:10:14.000000 opal_server-0.7.6/opal_server/scopes/loader.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1325 2023-05-09 07:59:18.000000 opal_server-0.7.6/opal_server/scopes/scope_repository.py
--rw-r--r--   0 roekatz    (501) staff       (20)     8442 2024-03-19 14:53:02.000000 opal_server-0.7.6/opal_server/scopes/service.py
--rw-r--r--   0 roekatz    (501) staff       (20)     3104 2024-03-19 14:53:02.000000 opal_server-0.7.6/opal_server/scopes/task.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:49.206642 opal_server-0.7.6/opal_server/security/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal_server-0.7.6/opal_server/security/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1423 2023-05-09 07:59:18.000000 opal_server-0.7.6/opal_server/security/api.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1277 2022-12-08 13:40:17.000000 opal_server-0.7.6/opal_server/security/jwks.py
--rw-r--r--   0 roekatz    (501) staff       (20)    17339 2024-04-30 13:01:51.000000 opal_server-0.7.6/opal_server/server.py
--rw-r--r--   0 roekatz    (501) staff       (20)    12533 2023-06-18 09:47:49.000000 opal_server-0.7.6/opal_server/statistics.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2024-04-30 17:18:49.206885 opal_server-0.7.6/opal_server.egg-info/
--rw-r--r--   0 roekatz    (501) staff       (20)    10196 2024-04-30 17:18:49.000000 opal_server-0.7.6/opal_server.egg-info/PKG-INFO
--rw-r--r--   0 roekatz    (501) staff       (20)     1246 2024-04-30 17:18:49.000000 opal_server-0.7.6/opal_server.egg-info/SOURCES.txt
--rw-r--r--   0 roekatz    (501) staff       (20)        1 2024-04-30 17:18:49.000000 opal_server-0.7.6/opal_server.egg-info/dependency_links.txt
--rw-r--r--   0 roekatz    (501) staff       (20)       52 2024-04-30 17:18:49.000000 opal_server-0.7.6/opal_server.egg-info/entry_points.txt
--rw-r--r--   0 roekatz    (501) staff       (20)      497 2024-04-30 17:18:49.000000 opal_server-0.7.6/opal_server.egg-info/requires.txt
--rw-r--r--   0 roekatz    (501) staff       (20)       12 2024-04-30 17:18:49.000000 opal_server-0.7.6/opal_server.egg-info/top_level.txt
--rw-r--r--   0 roekatz    (501) staff       (20)       38 2024-04-30 17:18:49.207975 opal_server-0.7.6/setup.cfg
--rw-r--r--   0 roekatz    (501) staff       (20)     3031 2024-04-30 13:01:51.000000 opal_server-0.7.6/setup.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2024-06-03 13:38:17.211946 opal-server-0.7.7/
+-rw-r--r--   0 asafc      (501) staff       (20)     9387 2024-06-03 13:38:17.211735 opal-server-0.7.7/PKG-INFO
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2024-06-03 13:38:17.207410 opal-server-0.7.7/opal_server/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-server-0.7.7/opal_server/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     2136 2023-05-10 06:45:11.000000 opal-server-0.7.7/opal_server/cli.py
+-rw-r--r--   0 asafc      (501) staff       (20)    11336 2024-05-29 13:03:42.000000 opal-server-0.7.7/opal_server/config.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2024-06-03 13:38:17.208933 opal-server-0.7.7/opal_server/data/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-server-0.7.7/opal_server/data/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5303 2023-09-11 17:35:10.000000 opal-server-0.7.7/opal_server/data/api.py
+-rw-r--r--   0 asafc      (501) staff       (20)     4004 2024-05-29 13:03:42.000000 opal-server-0.7.7/opal_server/data/data_update_publisher.py
+-rw-r--r--   0 asafc      (501) staff       (20)    15201 2024-03-17 08:56:30.000000 opal-server-0.7.7/opal_server/git_fetcher.py
+-rw-r--r--   0 asafc      (501) staff       (20)      987 2022-10-01 21:13:25.000000 opal-server-0.7.7/opal_server/loadlimiting.py
+-rw-r--r--   0 asafc      (501) staff       (20)      153 2022-10-01 21:13:25.000000 opal-server-0.7.7/opal_server/main.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2024-06-03 13:38:17.209077 opal-server-0.7.7/opal_server/policy/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-server-0.7.7/opal_server/policy/__init__.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2024-06-03 13:38:17.209283 opal-server-0.7.7/opal_server/policy/bundles/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-server-0.7.7/opal_server/policy/bundles/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     4447 2023-05-10 17:44:40.000000 opal-server-0.7.7/opal_server/policy/bundles/api.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2024-06-03 13:38:17.209850 opal-server-0.7.7/opal_server/policy/watcher/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2023-05-10 06:45:11.000000 opal-server-0.7.7/opal_server/policy/watcher/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     4529 2023-09-11 17:35:10.000000 opal-server-0.7.7/opal_server/policy/watcher/callbacks.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6662 2024-05-29 13:03:42.000000 opal-server-0.7.7/opal_server/policy/watcher/factory.py
+-rw-r--r--   0 asafc      (501) staff       (20)     4767 2023-09-11 17:35:10.000000 opal-server-0.7.7/opal_server/policy/watcher/task.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2024-06-03 13:38:17.210407 opal-server-0.7.7/opal_server/policy/webhook/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-server-0.7.7/opal_server/policy/webhook/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5690 2024-03-17 08:56:30.000000 opal-server-0.7.7/opal_server/policy/webhook/api.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6110 2023-02-24 20:59:56.000000 opal-server-0.7.7/opal_server/policy/webhook/deps.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1234 2022-10-01 21:13:25.000000 opal-server-0.7.7/opal_server/policy/webhook/listener.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1331 2022-10-01 21:13:25.000000 opal-server-0.7.7/opal_server/publisher.py
+-rw-r--r--   0 asafc      (501) staff       (20)     8009 2024-03-17 08:56:30.000000 opal-server-0.7.7/opal_server/pubsub.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1404 2023-10-24 07:43:19.000000 opal-server-0.7.7/opal_server/redis.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2024-06-03 13:38:17.211190 opal-server-0.7.7/opal_server/scopes/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-server-0.7.7/opal_server/scopes/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)    12784 2024-03-17 08:56:30.000000 opal-server-0.7.7/opal_server/scopes/api.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1621 2023-05-10 06:45:11.000000 opal-server-0.7.7/opal_server/scopes/loader.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1325 2022-10-11 10:23:16.000000 opal-server-0.7.7/opal_server/scopes/scope_repository.py
+-rw-r--r--   0 asafc      (501) staff       (20)     8442 2024-03-17 08:56:30.000000 opal-server-0.7.7/opal_server/scopes/service.py
+-rw-r--r--   0 asafc      (501) staff       (20)     3104 2024-03-17 08:56:30.000000 opal-server-0.7.7/opal_server/scopes/task.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2024-06-03 13:38:17.211515 opal-server-0.7.7/opal_server/security/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-server-0.7.7/opal_server/security/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1423 2022-10-11 10:23:16.000000 opal-server-0.7.7/opal_server/security/api.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1277 2022-10-01 21:13:25.000000 opal-server-0.7.7/opal_server/security/jwks.py
+-rw-r--r--   0 asafc      (501) staff       (20)    17339 2024-05-29 13:03:42.000000 opal-server-0.7.7/opal_server/server.py
+-rw-r--r--   0 asafc      (501) staff       (20)    12533 2023-02-01 11:46:28.000000 opal-server-0.7.7/opal_server/statistics.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2024-06-03 13:38:17.208442 opal-server-0.7.7/opal_server.egg-info/
+-rw-r--r--   0 asafc      (501) staff       (20)     9387 2024-06-03 13:38:17.000000 opal-server-0.7.7/opal_server.egg-info/PKG-INFO
+-rw-r--r--   0 asafc      (501) staff       (20)     1246 2024-06-03 13:38:17.000000 opal-server-0.7.7/opal_server.egg-info/SOURCES.txt
+-rw-r--r--   0 asafc      (501) staff       (20)        1 2024-06-03 13:38:17.000000 opal-server-0.7.7/opal_server.egg-info/dependency_links.txt
+-rw-r--r--   0 asafc      (501) staff       (20)       52 2024-06-03 13:38:17.000000 opal-server-0.7.7/opal_server.egg-info/entry_points.txt
+-rw-r--r--   0 asafc      (501) staff       (20)      497 2024-06-03 13:38:17.000000 opal-server-0.7.7/opal_server.egg-info/requires.txt
+-rw-r--r--   0 asafc      (501) staff       (20)       12 2024-06-03 13:38:17.000000 opal-server-0.7.7/opal_server.egg-info/top_level.txt
+-rw-r--r--   0 asafc      (501) staff       (20)       38 2024-06-03 13:38:17.211989 opal-server-0.7.7/setup.cfg
+-rw-r--r--   0 asafc      (501) staff       (20)     3031 2024-05-29 13:03:42.000000 opal-server-0.7.7/setup.py
```

### Comparing `opal_server-0.7.6/PKG-INFO` & `opal-server-0.7.7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opal-server
-Version: 0.7.6
+Version: 0.7.7
 Summary: OPAL is an administration layer for Open Policy Agent (OPA), detecting changes to both policy and data and pushing live updates to your agents. The opal-server creates a pub/sub channel clients can subscribe to (i.e: acts as coordinator). The server also tracks a git repository (via webhook) for updates to policy (or static data) and accepts continuous data update notifications via REST api, which are then pushed to clients.
 Home-page: https://github.com/permitio/opal
 Author: Or Weis, Asaf Cohen
 Author-email: or@permit.io
 License: Apache 2.0
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
@@ -14,35 +14,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: click<9,>=8.1.3
-Requires-Dist: permit-broadcaster[kafka,postgres,redis]==0.2.5
-Requires-Dist: gitpython<4,>=3.1.32
-Requires-Dist: pyjwt[crypto]<3,>=2.1.0
-Requires-Dist: websockets<11,>=10.3
-Requires-Dist: slowapi<1,>=0.1.5
-Requires-Dist: pygit2<2,>=1.13.3
-Requires-Dist: asgiref<4,>=3.5.2
-Requires-Dist: redis<5,>=4.3.4
-Requires-Dist: opal-common==0.7.6
-Requires-Dist: idna<4,>=3.3
-Requires-Dist: typer<1,>=0.4.1
-Requires-Dist: fastapi<1,>=0.109.1
-Requires-Dist: fastapi_websocket_pubsub==0.3.7
-Requires-Dist: fastapi_websocket_rpc<1,>=0.1.21
-Requires-Dist: gunicorn<23,>=22.0.0
-Requires-Dist: pydantic[email]<2,>=1.9.1
-Requires-Dist: typing-extensions; python_version < "3.8"
-Requires-Dist: uvicorn[standard]<1,>=0.17.6
-Requires-Dist: fastapi-utils<1,>=0.2.1
-Requires-Dist: setuptools>=65.5.1
 
 <p  align="center">
  <img src="https://github.com/permitio/opal/assets/4082578/4e21f85f-30ab-43e2-92de-b82f78888c71" height=170 alt="opal" border="0" />
 </p>
 <h1 align="center">
 ⚡OPAL⚡
 </h1>
```

#### html2text {}

```diff
@@ -1,34 +1,23 @@
-Metadata-Version: 2.1 Name: opal-server Version: 0.7.6 Summary: OPAL is an
+Metadata-Version: 2.1 Name: opal-server Version: 0.7.7 Summary: OPAL is an
 administration layer for Open Policy Agent (OPA), detecting changes to both
 policy and data and pushing live updates to your agents. The opal-server
 creates a pub/sub channel clients can subscribe to (i.e: acts as coordinator).
 The server also tracks a git repository (via webhook) for updates to policy (or
 static data) and accepts continuous data update notifications via REST api,
 which are then pushed to clients. Home-page: https://github.com/permitio/opal
 Author: Or Weis, Asaf Cohen Author-email: or@permit.io License: Apache 2.0
 Classifier: Operating System :: OS Independent Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP
 Servers Classifier: Topic :: Internet :: WWW/HTTP :: WSGI Requires-Python:
->=3.9 Description-Content-Type: text/markdown Requires-Dist: click<9,>=8.1.3
-Requires-Dist: permit-broadcaster[kafka,postgres,redis]==0.2.5 Requires-Dist:
-gitpython<4,>=3.1.32 Requires-Dist: pyjwt[crypto]<3,>=2.1.0 Requires-Dist:
-websockets<11,>=10.3 Requires-Dist: slowapi<1,>=0.1.5 Requires-Dist:
-pygit2<2,>=1.13.3 Requires-Dist: asgiref<4,>=3.5.2 Requires-Dist:
-redis<5,>=4.3.4 Requires-Dist: opal-common==0.7.6 Requires-Dist: idna<4,>=3.3
-Requires-Dist: typer<1,>=0.4.1 Requires-Dist: fastapi<1,>=0.109.1 Requires-
-Dist: fastapi_websocket_pubsub==0.3.7 Requires-Dist:
-fastapi_websocket_rpc<1,>=0.1.21 Requires-Dist: gunicorn<23,>=22.0.0 Requires-
-Dist: pydantic[email]<2,>=1.9.1 Requires-Dist: typing-extensions;
-python_version < "3.8" Requires-Dist: uvicorn[standard]<1,>=0.17.6 Requires-
-Dist: fastapi-utils<1,>=0.2.1 Requires-Dist: setuptools>=65.5.1
+>=3.9 Description-Content-Type: text/markdown
                                     [opal]
                            ************ ?â??¡OOPPAALL?â??¡ ************
                  ********** OOppeenn PPoolliiccyy AAddmmiinniissttrraattiioonn LLaayyeerr **********
 _[_T_e_s_t_s_]_[_P_a_c_k_a_g_e_]_[_P_a_c_k_a_g_e_]_[_D_o_w_n_l_o_a_d_s_]_[_D_o_c_k_e_r_ _p_u_l_l_s_]_[_J_o_i_n_ _o_u_r_ _S_l_a_c_k_!_]_[_h_t_t_p_s_:_/_/
 _i_m_g_._s_h_i_e_l_d_s_._i_o_/_t_w_i_t_t_e_r_/_f_o_l_l_o_w_/
 _p_e_r_m_i_t___i_o_?_l_a_b_e_l_=_F_o_l_l_o_w_%_2_0_%_4_0_p_e_r_m_i_t___i_o_&_s_t_y_l_e_=_s_o_c_i_a_l_]## What is OPAL? OPAL is an
 administration layer for Policy Engines such as _O_p_e_n_ _P_o_l_i_c_y_ _A_g_e_n_t_ _(_O_P_A_), and
```

### Comparing `opal_server-0.7.6/opal_server/cli.py` & `opal-server-0.7.7/opal_server/cli.py`

 * *Files identical despite different names*

### Comparing `opal_server-0.7.6/opal_server/config.py` & `opal-server-0.7.7/opal_server/config.py`

 * *Files identical despite different names*

### Comparing `opal_server-0.7.6/opal_server/data/api.py` & `opal-server-0.7.7/opal_server/data/api.py`

 * *Files identical despite different names*

### Comparing `opal_server-0.7.6/opal_server/data/data_update_publisher.py` & `opal-server-0.7.7/opal_server/data/data_update_publisher.py`

 * *Files identical despite different names*

### Comparing `opal_server-0.7.6/opal_server/git_fetcher.py` & `opal-server-0.7.7/opal_server/git_fetcher.py`

 * *Files identical despite different names*

### Comparing `opal_server-0.7.6/opal_server/loadlimiting.py` & `opal-server-0.7.7/opal_server/loadlimiting.py`

 * *Files identical despite different names*

### Comparing `opal_server-0.7.6/opal_server/policy/bundles/api.py` & `opal-server-0.7.7/opal_server/policy/bundles/api.py`

 * *Files identical despite different names*

### Comparing `opal_server-0.7.6/opal_server/policy/watcher/callbacks.py` & `opal-server-0.7.7/opal_server/policy/watcher/callbacks.py`

 * *Files identical despite different names*

### Comparing `opal_server-0.7.6/opal_server/policy/watcher/factory.py` & `opal-server-0.7.7/opal_server/policy/watcher/factory.py`

 * *Files identical despite different names*

### Comparing `opal_server-0.7.6/opal_server/policy/watcher/task.py` & `opal-server-0.7.7/opal_server/policy/watcher/task.py`

 * *Files identical despite different names*

### Comparing `opal_server-0.7.6/opal_server/policy/webhook/api.py` & `opal-server-0.7.7/opal_server/policy/webhook/api.py`

 * *Files identical despite different names*

### Comparing `opal_server-0.7.6/opal_server/policy/webhook/deps.py` & `opal-server-0.7.7/opal_server/policy/webhook/deps.py`

 * *Files identical despite different names*

### Comparing `opal_server-0.7.6/opal_server/policy/webhook/listener.py` & `opal-server-0.7.7/opal_server/policy/webhook/listener.py`

 * *Files identical despite different names*

### Comparing `opal_server-0.7.6/opal_server/publisher.py` & `opal-server-0.7.7/opal_server/publisher.py`

 * *Files identical despite different names*

### Comparing `opal_server-0.7.6/opal_server/pubsub.py` & `opal-server-0.7.7/opal_server/pubsub.py`

 * *Files identical despite different names*

### Comparing `opal_server-0.7.6/opal_server/redis.py` & `opal-server-0.7.7/opal_server/redis.py`

 * *Files identical despite different names*

### Comparing `opal_server-0.7.6/opal_server/scopes/api.py` & `opal-server-0.7.7/opal_server/scopes/api.py`

 * *Files identical despite different names*

### Comparing `opal_server-0.7.6/opal_server/scopes/loader.py` & `opal-server-0.7.7/opal_server/scopes/loader.py`

 * *Files identical despite different names*

### Comparing `opal_server-0.7.6/opal_server/scopes/scope_repository.py` & `opal-server-0.7.7/opal_server/scopes/scope_repository.py`

 * *Files identical despite different names*

### Comparing `opal_server-0.7.6/opal_server/scopes/service.py` & `opal-server-0.7.7/opal_server/scopes/service.py`

 * *Files identical despite different names*

### Comparing `opal_server-0.7.6/opal_server/scopes/task.py` & `opal-server-0.7.7/opal_server/scopes/task.py`

 * *Files identical despite different names*

### Comparing `opal_server-0.7.6/opal_server/security/api.py` & `opal-server-0.7.7/opal_server/security/api.py`

 * *Files identical despite different names*

### Comparing `opal_server-0.7.6/opal_server/security/jwks.py` & `opal-server-0.7.7/opal_server/security/jwks.py`

 * *Files identical despite different names*

### Comparing `opal_server-0.7.6/opal_server/server.py` & `opal-server-0.7.7/opal_server/server.py`

 * *Files identical despite different names*

### Comparing `opal_server-0.7.6/opal_server/statistics.py` & `opal-server-0.7.7/opal_server/statistics.py`

 * *Files identical despite different names*

### Comparing `opal_server-0.7.6/opal_server.egg-info/PKG-INFO` & `opal-server-0.7.7/opal_server.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opal-server
-Version: 0.7.6
+Version: 0.7.7
 Summary: OPAL is an administration layer for Open Policy Agent (OPA), detecting changes to both policy and data and pushing live updates to your agents. The opal-server creates a pub/sub channel clients can subscribe to (i.e: acts as coordinator). The server also tracks a git repository (via webhook) for updates to policy (or static data) and accepts continuous data update notifications via REST api, which are then pushed to clients.
 Home-page: https://github.com/permitio/opal
 Author: Or Weis, Asaf Cohen
 Author-email: or@permit.io
 License: Apache 2.0
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
@@ -14,35 +14,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: click<9,>=8.1.3
-Requires-Dist: permit-broadcaster[kafka,postgres,redis]==0.2.5
-Requires-Dist: gitpython<4,>=3.1.32
-Requires-Dist: pyjwt[crypto]<3,>=2.1.0
-Requires-Dist: websockets<11,>=10.3
-Requires-Dist: slowapi<1,>=0.1.5
-Requires-Dist: pygit2<2,>=1.13.3
-Requires-Dist: asgiref<4,>=3.5.2
-Requires-Dist: redis<5,>=4.3.4
-Requires-Dist: opal-common==0.7.6
-Requires-Dist: idna<4,>=3.3
-Requires-Dist: typer<1,>=0.4.1
-Requires-Dist: fastapi<1,>=0.109.1
-Requires-Dist: fastapi_websocket_pubsub==0.3.7
-Requires-Dist: fastapi_websocket_rpc<1,>=0.1.21
-Requires-Dist: gunicorn<23,>=22.0.0
-Requires-Dist: pydantic[email]<2,>=1.9.1
-Requires-Dist: typing-extensions; python_version < "3.8"
-Requires-Dist: uvicorn[standard]<1,>=0.17.6
-Requires-Dist: fastapi-utils<1,>=0.2.1
-Requires-Dist: setuptools>=65.5.1
 
 <p  align="center">
  <img src="https://github.com/permitio/opal/assets/4082578/4e21f85f-30ab-43e2-92de-b82f78888c71" height=170 alt="opal" border="0" />
 </p>
 <h1 align="center">
 ⚡OPAL⚡
 </h1>
```

#### html2text {}

```diff
@@ -1,34 +1,23 @@
-Metadata-Version: 2.1 Name: opal-server Version: 0.7.6 Summary: OPAL is an
+Metadata-Version: 2.1 Name: opal-server Version: 0.7.7 Summary: OPAL is an
 administration layer for Open Policy Agent (OPA), detecting changes to both
 policy and data and pushing live updates to your agents. The opal-server
 creates a pub/sub channel clients can subscribe to (i.e: acts as coordinator).
 The server also tracks a git repository (via webhook) for updates to policy (or
 static data) and accepts continuous data update notifications via REST api,
 which are then pushed to clients. Home-page: https://github.com/permitio/opal
 Author: Or Weis, Asaf Cohen Author-email: or@permit.io License: Apache 2.0
 Classifier: Operating System :: OS Independent Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP
 Servers Classifier: Topic :: Internet :: WWW/HTTP :: WSGI Requires-Python:
->=3.9 Description-Content-Type: text/markdown Requires-Dist: click<9,>=8.1.3
-Requires-Dist: permit-broadcaster[kafka,postgres,redis]==0.2.5 Requires-Dist:
-gitpython<4,>=3.1.32 Requires-Dist: pyjwt[crypto]<3,>=2.1.0 Requires-Dist:
-websockets<11,>=10.3 Requires-Dist: slowapi<1,>=0.1.5 Requires-Dist:
-pygit2<2,>=1.13.3 Requires-Dist: asgiref<4,>=3.5.2 Requires-Dist:
-redis<5,>=4.3.4 Requires-Dist: opal-common==0.7.6 Requires-Dist: idna<4,>=3.3
-Requires-Dist: typer<1,>=0.4.1 Requires-Dist: fastapi<1,>=0.109.1 Requires-
-Dist: fastapi_websocket_pubsub==0.3.7 Requires-Dist:
-fastapi_websocket_rpc<1,>=0.1.21 Requires-Dist: gunicorn<23,>=22.0.0 Requires-
-Dist: pydantic[email]<2,>=1.9.1 Requires-Dist: typing-extensions;
-python_version < "3.8" Requires-Dist: uvicorn[standard]<1,>=0.17.6 Requires-
-Dist: fastapi-utils<1,>=0.2.1 Requires-Dist: setuptools>=65.5.1
+>=3.9 Description-Content-Type: text/markdown
                                     [opal]
                            ************ ?â??¡OOPPAALL?â??¡ ************
                  ********** OOppeenn PPoolliiccyy AAddmmiinniissttrraattiioonn LLaayyeerr **********
 _[_T_e_s_t_s_]_[_P_a_c_k_a_g_e_]_[_P_a_c_k_a_g_e_]_[_D_o_w_n_l_o_a_d_s_]_[_D_o_c_k_e_r_ _p_u_l_l_s_]_[_J_o_i_n_ _o_u_r_ _S_l_a_c_k_!_]_[_h_t_t_p_s_:_/_/
 _i_m_g_._s_h_i_e_l_d_s_._i_o_/_t_w_i_t_t_e_r_/_f_o_l_l_o_w_/
 _p_e_r_m_i_t___i_o_?_l_a_b_e_l_=_F_o_l_l_o_w_%_2_0_%_4_0_p_e_r_m_i_t___i_o_&_s_t_y_l_e_=_s_o_c_i_a_l_]## What is OPAL? OPAL is an
 administration layer for Policy Engines such as _O_p_e_n_ _P_o_l_i_c_y_ _A_g_e_n_t_ _(_O_P_A_), and
```

### Comparing `opal_server-0.7.6/opal_server.egg-info/SOURCES.txt` & `opal-server-0.7.7/opal_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opal_server-0.7.6/setup.py` & `opal-server-0.7.7/setup.py`

 * *Files identical despite different names*

