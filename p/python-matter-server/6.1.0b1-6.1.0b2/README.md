# Comparing `tmp/python_matter_server-6.1.0b1.tar.gz` & `tmp/python_matter_server-6.1.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_matter_server-6.1.0b1.tar", last modified: Wed May 29 15:15:39 2024, max compression
+gzip compressed data, was "python_matter_server-6.1.0b2.tar", last modified: Mon Jun  3 11:18:31 2024, max compression
```

## Comparing `python_matter_server-6.1.0b1.tar` & `python_matter_server-6.1.0b2.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:15:39.171234 python_matter_server-6.1.0b1/
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-29 15:15:24.000000 python_matter_server-6.1.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14206 2024-05-29 15:15:39.171234 python_matter_server-6.1.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12409 2024-05-29 15:15:24.000000 python_matter_server-6.1.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:15:39.163234 python_matter_server-6.1.0b1/matter_server/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-29 15:15:24.000000 python_matter_server-6.1.0b1/matter_server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:15:39.163234 python_matter_server-6.1.0b1/matter_server/client/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-29 15:15:24.000000 python_matter_server-6.1.0b1/matter_server/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29159 2024-05-29 15:15:24.000000 python_matter_server-6.1.0b1/matter_server/client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5757 2024-05-29 15:15:24.000000 python_matter_server-6.1.0b1/matter_server/client/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-29 15:15:24.000000 python_matter_server-6.1.0b1/matter_server/client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:15:39.163234 python_matter_server-6.1.0b1/matter_server/client/models/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-29 15:15:24.000000 python_matter_server-6.1.0b1/matter_server/client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21263 2024-05-29 15:15:24.000000 python_matter_server-6.1.0b1/matter_server/client/models/device_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    15226 2024-05-29 15:15:24.000000 python_matter_server-6.1.0b1/matter_server/client/models/node.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:15:39.163234 python_matter_server-6.1.0b1/matter_server/common/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-29 15:15:24.000000 python_matter_server-6.1.0b1/matter_server/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-29 15:15:24.000000 python_matter_server-6.1.0b1/matter_server/common/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     7778 2024-05-29 15:15:24.000000 python_matter_server-6.1.0b1/matter_server/common/custom_clusters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-29 15:15:24.000000 python_matter_server-6.1.0b1/matter_server/common/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:15:39.163234 python_matter_server-6.1.0b1/matter_server/common/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-29 15:15:24.000000 python_matter_server-6.1.0b1/matter_server/common/helpers/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-29 15:15:24.000000 python_matter_server-6.1.0b1/matter_server/common/helpers/json.py
--rw-r--r--   0 runner    (1001) docker     (127)    12201 2024-05-29 15:15:24.000000 python_matter_server-6.1.0b1/matter_server/common/helpers/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-05-29 15:15:24.000000 python_matter_server-6.1.0b1/matter_server/common/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:15:39.163234 python_matter_server-6.1.0b1/matter_server/dashboard/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-29 15:15:37.000000 python_matter_server-6.1.0b1/matter_server/dashboard/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:15:39.163234 python_matter_server-6.1.0b1/matter_server/dashboard/js/
--rw-r--r--   0 runner    (1001) docker     (127)    13016 2024-05-29 15:15:36.000000 python_matter_server-6.1.0b1/matter_server/dashboard/js/dialog-box-DTRaWTo2.js
--rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-05-29 15:15:36.000000 python_matter_server-6.1.0b1/matter_server/dashboard/js/main.js
--rw-r--r--   0 runner    (1001) docker     (127)   255440 2024-05-29 15:15:36.000000 python_matter_server-6.1.0b1/matter_server/dashboard/js/matter-dashboard-app-pMm2fVnD.js
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 15:15:24.000000 python_matter_server-6.1.0b1/matter_server/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:15:39.167234 python_matter_server-6.1.0b1/matter_server/server/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-29 15:15:24.000000 python_matter_server-6.1.0b1/matter_server/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-05-29 15:15:24.000000 python_matter_server-6.1.0b1/matter_server/server/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9307 2024-05-29 15:15:24.000000 python_matter_server-6.1.0b1/matter_server/server/client_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-29 15:15:24.000000 python_matter_server-6.1.0b1/matter_server/server/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    60523 2024-05-29 15:15:24.000000 python_matter_server-6.1.0b1/matter_server/server/device_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:15:39.167234 python_matter_server-6.1.0b1/matter_server/server/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-29 15:15:24.000000 python_matter_server-6.1.0b1/matter_server/server/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-29 15:15:24.000000 python_matter_server-6.1.0b1/matter_server/server/helpers/attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-05-29 15:15:24.000000 python_matter_server-6.1.0b1/matter_server/server/helpers/custom_web_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     9147 2024-05-29 15:15:24.000000 python_matter_server-6.1.0b1/matter_server/server/helpers/paa_certificates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-29 15:15:24.000000 python_matter_server-6.1.0b1/matter_server/server/helpers/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13468 2024-05-29 15:15:24.000000 python_matter_server-6.1.0b1/matter_server/server/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)    11913 2024-05-29 15:15:24.000000 python_matter_server-6.1.0b1/matter_server/server/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-05-29 15:15:24.000000 python_matter_server-6.1.0b1/matter_server/server/stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     5406 2024-05-29 15:15:24.000000 python_matter_server-6.1.0b1/matter_server/server/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-05-29 15:15:24.000000 python_matter_server-6.1.0b1/matter_server/server/vendor_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4781 2024-05-29 15:15:26.000000 python_matter_server-6.1.0b1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:15:39.167234 python_matter_server-6.1.0b1/python_matter_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14206 2024-05-29 15:15:39.000000 python_matter_server-6.1.0b1/python_matter_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-29 15:15:39.000000 python_matter_server-6.1.0b1/python_matter_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 15:15:39.000000 python_matter_server-6.1.0b1/python_matter_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-29 15:15:39.000000 python_matter_server-6.1.0b1/python_matter_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 15:15:38.000000 python_matter_server-6.1.0b1/python_matter_server.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-29 15:15:39.000000 python_matter_server-6.1.0b1/python_matter_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-29 15:15:39.000000 python_matter_server-6.1.0b1/python_matter_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 15:15:39.171234 python_matter_server-6.1.0b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:18:31.756840 python_matter_server-6.1.0b2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-06-03 11:18:17.000000 python_matter_server-6.1.0b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14206 2024-06-03 11:18:31.756840 python_matter_server-6.1.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12409 2024-06-03 11:18:17.000000 python_matter_server-6.1.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:18:31.748840 python_matter_server-6.1.0b2/matter_server/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-06-03 11:18:17.000000 python_matter_server-6.1.0b2/matter_server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:18:31.748840 python_matter_server-6.1.0b2/matter_server/client/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-06-03 11:18:17.000000 python_matter_server-6.1.0b2/matter_server/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29159 2024-06-03 11:18:17.000000 python_matter_server-6.1.0b2/matter_server/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5757 2024-06-03 11:18:17.000000 python_matter_server-6.1.0b2/matter_server/client/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-06-03 11:18:17.000000 python_matter_server-6.1.0b2/matter_server/client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:18:31.748840 python_matter_server-6.1.0b2/matter_server/client/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-06-03 11:18:17.000000 python_matter_server-6.1.0b2/matter_server/client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21263 2024-06-03 11:18:17.000000 python_matter_server-6.1.0b2/matter_server/client/models/device_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15226 2024-06-03 11:18:17.000000 python_matter_server-6.1.0b2/matter_server/client/models/node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:18:31.748840 python_matter_server-6.1.0b2/matter_server/common/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-06-03 11:18:17.000000 python_matter_server-6.1.0b2/matter_server/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-06-03 11:18:17.000000 python_matter_server-6.1.0b2/matter_server/common/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7778 2024-06-03 11:18:17.000000 python_matter_server-6.1.0b2/matter_server/common/custom_clusters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-06-03 11:18:17.000000 python_matter_server-6.1.0b2/matter_server/common/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:18:31.748840 python_matter_server-6.1.0b2/matter_server/common/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-06-03 11:18:17.000000 python_matter_server-6.1.0b2/matter_server/common/helpers/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-06-03 11:18:17.000000 python_matter_server-6.1.0b2/matter_server/common/helpers/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12201 2024-06-03 11:18:17.000000 python_matter_server-6.1.0b2/matter_server/common/helpers/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-06-03 11:18:17.000000 python_matter_server-6.1.0b2/matter_server/common/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:18:31.748840 python_matter_server-6.1.0b2/matter_server/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-06-03 11:18:29.000000 python_matter_server-6.1.0b2/matter_server/dashboard/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:18:31.752840 python_matter_server-6.1.0b2/matter_server/dashboard/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    13016 2024-06-03 11:18:29.000000 python_matter_server-6.1.0b2/matter_server/dashboard/js/dialog-box-DTRaWTo2.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-06-03 11:18:29.000000 python_matter_server-6.1.0b2/matter_server/dashboard/js/main.js
+-rw-r--r--   0 runner    (1001) docker     (127)   255440 2024-06-03 11:18:29.000000 python_matter_server-6.1.0b2/matter_server/dashboard/js/matter-dashboard-app-pMm2fVnD.js
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:18:17.000000 python_matter_server-6.1.0b2/matter_server/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:18:31.752840 python_matter_server-6.1.0b2/matter_server/server/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-06-03 11:18:17.000000 python_matter_server-6.1.0b2/matter_server/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-06-03 11:18:17.000000 python_matter_server-6.1.0b2/matter_server/server/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9307 2024-06-03 11:18:17.000000 python_matter_server-6.1.0b2/matter_server/server/client_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-06-03 11:18:17.000000 python_matter_server-6.1.0b2/matter_server/server/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60574 2024-06-03 11:18:17.000000 python_matter_server-6.1.0b2/matter_server/server/device_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:18:31.752840 python_matter_server-6.1.0b2/matter_server/server/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-06-03 11:18:17.000000 python_matter_server-6.1.0b2/matter_server/server/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-06-03 11:18:17.000000 python_matter_server-6.1.0b2/matter_server/server/helpers/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-06-03 11:18:17.000000 python_matter_server-6.1.0b2/matter_server/server/helpers/custom_web_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9147 2024-06-03 11:18:17.000000 python_matter_server-6.1.0b2/matter_server/server/helpers/paa_certificates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-06-03 11:18:17.000000 python_matter_server-6.1.0b2/matter_server/server/helpers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14190 2024-06-03 11:18:17.000000 python_matter_server-6.1.0b2/matter_server/server/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11913 2024-06-03 11:18:17.000000 python_matter_server-6.1.0b2/matter_server/server/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-06-03 11:18:17.000000 python_matter_server-6.1.0b2/matter_server/server/stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5406 2024-06-03 11:18:17.000000 python_matter_server-6.1.0b2/matter_server/server/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-06-03 11:18:17.000000 python_matter_server-6.1.0b2/matter_server/server/vendor_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4781 2024-06-03 11:18:19.000000 python_matter_server-6.1.0b2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:18:31.756840 python_matter_server-6.1.0b2/python_matter_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14206 2024-06-03 11:18:31.000000 python_matter_server-6.1.0b2/python_matter_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-06-03 11:18:31.000000 python_matter_server-6.1.0b2/python_matter_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 11:18:31.000000 python_matter_server-6.1.0b2/python_matter_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-06-03 11:18:31.000000 python_matter_server-6.1.0b2/python_matter_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 11:18:31.000000 python_matter_server-6.1.0b2/python_matter_server.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-06-03 11:18:31.000000 python_matter_server-6.1.0b2/python_matter_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-06-03 11:18:31.000000 python_matter_server-6.1.0b2/python_matter_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 11:18:31.756840 python_matter_server-6.1.0b2/setup.cfg
```

### Comparing `python_matter_server-6.1.0b1/LICENSE` & `python_matter_server-6.1.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.1.0b1/PKG-INFO` & `python_matter_server-6.1.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-matter-server
-Version: 6.1.0b1
+Version: 6.1.0b2
 Summary: Python Matter WebSocket Server
 Author-email: The Home Assistant Authors <hello@home-assistant.io>
 License: Apache-2.0
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
@@ -15,36 +15,36 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp
 Requires-Dist: aiorun
 Requires-Dist: async-timeout
 Requires-Dist: coloredlogs
 Requires-Dist: orjson
-Requires-Dist: home-assistant-chip-clusters==2024.5.1
+Requires-Dist: home-assistant-chip-clusters==2024.5.2
 Provides-Extra: server
 Requires-Dist: aiohttp==3.9.5; extra == "server"
 Requires-Dist: aiorun==2024.5.1; extra == "server"
 Requires-Dist: async-timeout==4.0.3; extra == "server"
 Requires-Dist: coloredlogs==15.0.1; extra == "server"
 Requires-Dist: cryptography==42.0.7; extra == "server"
 Requires-Dist: orjson==3.10.3; extra == "server"
 Requires-Dist: zeroconf==0.132.2; extra == "server"
-Requires-Dist: home-assistant-chip-core==2024.5.1; extra == "server"
+Requires-Dist: home-assistant-chip-core==2024.5.2; extra == "server"
 Provides-Extra: test
 Requires-Dist: codespell==2.3.0; extra == "test"
 Requires-Dist: isort==5.13.2; extra == "test"
 Requires-Dist: mypy==1.10.0; extra == "test"
 Requires-Dist: pre-commit==3.7.1; extra == "test"
 Requires-Dist: pre-commit-hooks==4.6.0; extra == "test"
 Requires-Dist: pylint==3.2.2; extra == "test"
 Requires-Dist: pytest==8.2.1; extra == "test"
 Requires-Dist: pytest-asyncio==0.23.7; extra == "test"
 Requires-Dist: pytest-aiohttp==1.0.5; extra == "test"
 Requires-Dist: pytest-cov==5.0.0; extra == "test"
-Requires-Dist: ruff==0.4.5; extra == "test"
+Requires-Dist: ruff==0.4.7; extra == "test"
 Requires-Dist: tomli==2.0.1; extra == "test"
 
 # Python Matter Server
 
 This project implements a Matter Controller Server over WebSockets using the
 [official Matter (formerly CHIP) SDK](https://github.com/project-chip/connectedhomeip)
 as a base and provides both a server and client implementation.
```

### Comparing `python_matter_server-6.1.0b1/README.md` & `python_matter_server-6.1.0b2/README.md`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.1.0b1/matter_server/client/client.py` & `python_matter_server-6.1.0b2/matter_server/client/client.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.1.0b1/matter_server/client/connection.py` & `python_matter_server-6.1.0b2/matter_server/client/connection.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.1.0b1/matter_server/client/exceptions.py` & `python_matter_server-6.1.0b2/matter_server/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.1.0b1/matter_server/client/models/device_types.py` & `python_matter_server-6.1.0b2/matter_server/client/models/device_types.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.1.0b1/matter_server/client/models/node.py` & `python_matter_server-6.1.0b2/matter_server/client/models/node.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.1.0b1/matter_server/common/custom_clusters.py` & `python_matter_server-6.1.0b2/matter_server/common/custom_clusters.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.1.0b1/matter_server/common/errors.py` & `python_matter_server-6.1.0b2/matter_server/common/errors.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.1.0b1/matter_server/common/helpers/api.py` & `python_matter_server-6.1.0b2/matter_server/common/helpers/api.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.1.0b1/matter_server/common/helpers/json.py` & `python_matter_server-6.1.0b2/matter_server/common/helpers/json.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.1.0b1/matter_server/common/helpers/util.py` & `python_matter_server-6.1.0b2/matter_server/common/helpers/util.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.1.0b1/matter_server/common/models.py` & `python_matter_server-6.1.0b2/matter_server/common/models.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.1.0b1/matter_server/dashboard/index.html` & `python_matter_server-6.1.0b2/matter_server/dashboard/index.html`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.1.0b1/matter_server/dashboard/js/dialog-box-DTRaWTo2.js` & `python_matter_server-6.1.0b2/matter_server/dashboard/js/dialog-box-DTRaWTo2.js`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.1.0b1/matter_server/dashboard/js/main.js` & `python_matter_server-6.1.0b2/matter_server/dashboard/js/main.js`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.1.0b1/matter_server/dashboard/js/matter-dashboard-app-pMm2fVnD.js` & `python_matter_server-6.1.0b2/matter_server/dashboard/js/matter-dashboard-app-pMm2fVnD.js`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.1.0b1/matter_server/server/__main__.py` & `python_matter_server-6.1.0b2/matter_server/server/__main__.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.1.0b1/matter_server/server/client_handler.py` & `python_matter_server-6.1.0b2/matter_server/server/client_handler.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.1.0b1/matter_server/server/const.py` & `python_matter_server-6.1.0b2/matter_server/server/const.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.1.0b1/matter_server/server/device_controller.py` & `python_matter_server-6.1.0b2/matter_server/server/device_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -689,14 +689,15 @@
                 f"Node {node_id} does not exist or has not been interviewed."
             )
 
         LOGGER.info("Removing Node ID %s.", node_id)
 
         # shutdown any existing subscriptions
         await self._chip_device_controller.shutdown_subscription(node_id)
+        self._polled_attributes.pop(node_id, None)
 
         node = self._nodes.pop(node_id)
         self.server.storage.remove(
             DATA_KEY_NODES,
             subkey=str(node_id),
         )
```

### Comparing `python_matter_server-6.1.0b1/matter_server/server/helpers/attributes.py` & `python_matter_server-6.1.0b2/matter_server/server/helpers/attributes.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.1.0b1/matter_server/server/helpers/custom_web_runner.py` & `python_matter_server-6.1.0b2/matter_server/server/helpers/custom_web_runner.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.1.0b1/matter_server/server/helpers/paa_certificates.py` & `python_matter_server-6.1.0b2/matter_server/server/helpers/paa_certificates.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.1.0b1/matter_server/server/helpers/utils.py` & `python_matter_server-6.1.0b2/matter_server/server/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.1.0b1/matter_server/server/sdk.py` & `python_matter_server-6.1.0b2/matter_server/server/sdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 make the classes easier to use in asyncio environment and our use case in general. It
 also makes the API more pythonic where possible.
 """
 
 from __future__ import annotations
 
 import asyncio
+from concurrent.futures import ThreadPoolExecutor
 from functools import partial
 import logging
 import time
 from typing import TYPE_CHECKING, Any, TypeVar, cast
 
 from chip.clusters import Attribute, Objects as Clusters
 from chip.clusters.Attribute import AttributeWriteResult
@@ -54,45 +55,65 @@
 
     def __init__(self, server: MatterServer, paa_root_cert_dir: Path):
         """Initialize the device controller."""
         self.server = server
 
         self._node_lock: dict[int, asyncio.Lock] = {}
         self._subscriptions: dict[int, Attribute.SubscriptionTransaction] = {}
+        self._sdk_non_entrant_executor = ThreadPoolExecutor(max_workers=1)
 
         # Instantiate the underlying ChipDeviceController instance on the Fabric
         self._chip_controller = self.server.stack.fabric_admin.NewController(
             paaTrustStorePath=str(paa_root_cert_dir)
         )
         LOGGER.debug("CHIP Device Controller Initialized")
 
     def _get_node_lock(self, node_id: int) -> asyncio.Lock:
         """Return lock for given node."""
         if node_id not in self._node_lock:
             self._node_lock[node_id] = asyncio.Lock()
         return self._node_lock[node_id]
 
-    async def _call_sdk(
+    async def _call_sdk_executor(
         self,
+        executor: ThreadPoolExecutor | None,
         target: Callable[..., _T],
         *args: Any,
         **kwargs: Any,
     ) -> _T:
         """Call function on the SDK in executor and return result."""
         if self.server.loop is None:
             raise RuntimeError("Server not started.")
 
         return cast(
             _T,
             await self.server.loop.run_in_executor(
-                None,
+                executor,
                 partial(target, *args, **kwargs),
             ),
         )
 
+    async def _call_sdk(
+        self,
+        target: Callable[..., _T],
+        *args: Any,
+        **kwargs: Any,
+    ) -> _T:
+        return await self._call_sdk_executor(None, target, *args, **kwargs)
+
+    async def _call_sdk_non_reentrant(
+        self,
+        target: Callable[..., _T],
+        *args: Any,
+        **kwargs: Any,
+    ) -> _T:
+        return await self._call_sdk_executor(
+            self._sdk_non_entrant_executor, target, *args, **kwargs
+        )
+
     async def get_compressed_fabric_id(self) -> int:
         """Get the compressed fabric id."""
         return await self._call_sdk(self._chip_controller.GetCompressedFabricId)
 
     async def shutdown(self) -> None:
         """Shutdown the device controller."""
         # unsubscribe all node subscriptions
@@ -105,42 +126,42 @@
     async def commission_with_code(
         self,
         node_id: int,
         setup_payload: str,
         discovery_type: DiscoveryType,
     ) -> PyChipError:
         """Commission a device using a QR Code or Manual Pairing Code."""
-        return await self._call_sdk(
+        return await self._call_sdk_non_reentrant(
             self._chip_controller.CommissionWithCode,
             setupPayload=setup_payload,
             nodeid=node_id,
             discoveryType=discovery_type,
         )
 
     async def commission_on_network(
         self,
         node_id: int,
         setup_pin_code: int,
         disc_filter_type: FilterType = FilterType.NONE,
         disc_filter: Any = None,
     ) -> PyChipError:
         """Commission a device on the network."""
-        return await self._call_sdk(
+        return await self._call_sdk_non_reentrant(
             self._chip_controller.CommissionOnNetwork,
             nodeId=node_id,
             setupPinCode=setup_pin_code,
             filterType=disc_filter_type,
             filter=disc_filter,
         )
 
     async def commission_ip(
         self, node_id: int, setup_pin_code: int, ip_addr: str
     ) -> PyChipError:
         """Commission a device using an IP address."""
-        return await self._call_sdk(
+        return await self._call_sdk_non_reentrant(
             self._chip_controller.CommissionIP,
             nodeid=node_id,
             setupPinCode=setup_pin_code,
             ipaddr=ip_addr,
         )
 
     async def set_wifi_credentials(self, ssid: str, credentials: str) -> None:
@@ -164,15 +185,15 @@
         timeout: int,
         iteration: int,
         discriminator: int,
         option: ChipDeviceController.CommissioningWindowPasscode,
     ) -> CommissioningParameters:
         """Open a commissioning window to commission a device present on this controller to another."""
         async with self._get_node_lock(node_id):
-            await self._call_sdk(
+            return await self._call_sdk_non_reentrant(
                 self._chip_controller.OpenCommissioningWindow,
                 nodeid=node_id,
                 timeout=timeout,
                 iteration=iteration,
                 discriminator=discriminator,
                 option=option,
             )
```

### Comparing `python_matter_server-6.1.0b1/matter_server/server/server.py` & `python_matter_server-6.1.0b2/matter_server/server/server.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.1.0b1/matter_server/server/stack.py` & `python_matter_server-6.1.0b2/matter_server/server/stack.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.1.0b1/matter_server/server/storage.py` & `python_matter_server-6.1.0b2/matter_server/server/storage.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.1.0b1/matter_server/server/vendor_info.py` & `python_matter_server-6.1.0b2/matter_server/server/vendor_info.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.1.0b1/pyproject.toml` & `python_matter_server-6.1.0b2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -18,48 +18,48 @@
 ]
 dependencies = [
     "aiohttp",
     "aiorun",
     "async-timeout",
     "coloredlogs",
     "orjson",
-    "home-assistant-chip-clusters==2024.5.1",
+    "home-assistant-chip-clusters==2024.5.2",
 ]
 description = "Python Matter WebSocket Server"
 name = "python-matter-server"
 readme = "README.md"
 requires-python = ">=3.11"
-version = "6.1.0b1"
+version = "6.1.0b2"
 
 [project.license]
 text = "Apache-2.0"
 
 [project.optional-dependencies]
 server = [
     "aiohttp==3.9.5",
     "aiorun==2024.5.1",
     "async-timeout==4.0.3",
     "coloredlogs==15.0.1",
     "cryptography==42.0.7",
     "orjson==3.10.3",
     "zeroconf==0.132.2",
-    "home-assistant-chip-core==2024.5.1",
+    "home-assistant-chip-core==2024.5.2",
 ]
 test = [
     "codespell==2.3.0",
     "isort==5.13.2",
     "mypy==1.10.0",
     "pre-commit==3.7.1",
     "pre-commit-hooks==4.6.0",
     "pylint==3.2.2",
     "pytest==8.2.1",
     "pytest-asyncio==0.23.7",
     "pytest-aiohttp==1.0.5",
     "pytest-cov==5.0.0",
-    "ruff==0.4.5",
+    "ruff==0.4.7",
     "tomli==2.0.1",
 ]
 
 [project.scripts]
 matter-server = "matter_server.server.__main__:main"
 
 [tool.codespell]
```

### Comparing `python_matter_server-6.1.0b1/python_matter_server.egg-info/PKG-INFO` & `python_matter_server-6.1.0b2/python_matter_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-matter-server
-Version: 6.1.0b1
+Version: 6.1.0b2
 Summary: Python Matter WebSocket Server
 Author-email: The Home Assistant Authors <hello@home-assistant.io>
 License: Apache-2.0
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
@@ -15,36 +15,36 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp
 Requires-Dist: aiorun
 Requires-Dist: async-timeout
 Requires-Dist: coloredlogs
 Requires-Dist: orjson
-Requires-Dist: home-assistant-chip-clusters==2024.5.1
+Requires-Dist: home-assistant-chip-clusters==2024.5.2
 Provides-Extra: server
 Requires-Dist: aiohttp==3.9.5; extra == "server"
 Requires-Dist: aiorun==2024.5.1; extra == "server"
 Requires-Dist: async-timeout==4.0.3; extra == "server"
 Requires-Dist: coloredlogs==15.0.1; extra == "server"
 Requires-Dist: cryptography==42.0.7; extra == "server"
 Requires-Dist: orjson==3.10.3; extra == "server"
 Requires-Dist: zeroconf==0.132.2; extra == "server"
-Requires-Dist: home-assistant-chip-core==2024.5.1; extra == "server"
+Requires-Dist: home-assistant-chip-core==2024.5.2; extra == "server"
 Provides-Extra: test
 Requires-Dist: codespell==2.3.0; extra == "test"
 Requires-Dist: isort==5.13.2; extra == "test"
 Requires-Dist: mypy==1.10.0; extra == "test"
 Requires-Dist: pre-commit==3.7.1; extra == "test"
 Requires-Dist: pre-commit-hooks==4.6.0; extra == "test"
 Requires-Dist: pylint==3.2.2; extra == "test"
 Requires-Dist: pytest==8.2.1; extra == "test"
 Requires-Dist: pytest-asyncio==0.23.7; extra == "test"
 Requires-Dist: pytest-aiohttp==1.0.5; extra == "test"
 Requires-Dist: pytest-cov==5.0.0; extra == "test"
-Requires-Dist: ruff==0.4.5; extra == "test"
+Requires-Dist: ruff==0.4.7; extra == "test"
 Requires-Dist: tomli==2.0.1; extra == "test"
 
 # Python Matter Server
 
 This project implements a Matter Controller Server over WebSockets using the
 [official Matter (formerly CHIP) SDK](https://github.com/project-chip/connectedhomeip)
 as a base and provides both a server and client implementation.
```

### Comparing `python_matter_server-6.1.0b1/python_matter_server.egg-info/SOURCES.txt` & `python_matter_server-6.1.0b2/python_matter_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

