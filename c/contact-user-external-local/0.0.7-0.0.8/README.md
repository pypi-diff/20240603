# Comparing `tmp/contact_user_external_local-0.0.7.tar.gz` & `tmp/contact_user_external_local-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contact_user_external_local-0.0.7.tar", last modified: Sun May 26 23:32:34 2024, max compression
+gzip compressed data, was "contact_user_external_local-0.0.8.tar", last modified: Mon Jun  3 15:07:29 2024, max compression
```

## Comparing `contact_user_external_local-0.0.7.tar` & `contact_user_external_local-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:32:34.050302 contact_user_external_local-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-26 23:32:34.050302 contact_user_external_local-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-26 23:32:03.000000 contact_user_external_local-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:32:34.046302 contact_user_external_local-0.0.7/contact_user_external_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:32:34.050302 contact_user_external_local-0.0.7/contact_user_external_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 23:32:03.000000 contact_user_external_local-0.0.7/contact_user_external_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5998 2024-05-26 23:32:03.000000 contact_user_external_local-0.0.7/contact_user_external_local/src/contact_user_external_local.py
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-26 23:32:03.000000 contact_user_external_local-0.0.7/contact_user_external_local/src/contact_user_external_local_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:32:34.050302 contact_user_external_local-0.0.7/contact_user_external_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-26 23:32:34.000000 contact_user_external_local-0.0.7/contact_user_external_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-26 23:32:34.000000 contact_user_external_local-0.0.7/contact_user_external_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 23:32:34.000000 contact_user_external_local-0.0.7/contact_user_external_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-26 23:32:34.000000 contact_user_external_local-0.0.7/contact_user_external_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-26 23:32:34.000000 contact_user_external_local-0.0.7/contact_user_external_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-26 23:32:10.000000 contact_user_external_local-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 23:32:34.050302 contact_user_external_local-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-26 23:32:03.000000 contact_user_external_local-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:07:29.365564 contact_user_external_local-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-06-03 15:07:29.365564 contact_user_external_local-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-06-03 15:06:56.000000 contact_user_external_local-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:07:29.361564 contact_user_external_local-0.0.8/contact_user_external_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:07:29.365564 contact_user_external_local-0.0.8/contact_user_external_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:06:56.000000 contact_user_external_local-0.0.8/contact_user_external_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11895 2024-06-03 15:06:56.000000 contact_user_external_local-0.0.8/contact_user_external_local/src/contact_user_external_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-06-03 15:06:56.000000 contact_user_external_local-0.0.8/contact_user_external_local/src/contact_user_external_local_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:07:29.365564 contact_user_external_local-0.0.8/contact_user_external_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-06-03 15:07:29.000000 contact_user_external_local-0.0.8/contact_user_external_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-06-03 15:07:29.000000 contact_user_external_local-0.0.8/contact_user_external_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 15:07:29.000000 contact_user_external_local-0.0.8/contact_user_external_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-06-03 15:07:29.000000 contact_user_external_local-0.0.8/contact_user_external_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-06-03 15:07:29.000000 contact_user_external_local-0.0.8/contact_user_external_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-06-03 15:07:04.000000 contact_user_external_local-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 15:07:29.365564 contact_user_external_local-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-06-03 15:06:56.000000 contact_user_external_local-0.0.8/setup.py
```

### Comparing `contact_user_external_local-0.0.7/PKG-INFO` & `contact_user_external_local-0.0.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: contact-user-external-local
-Version: 0.0.7
+Version: 0.0.8
 Summary: PyPI Package for Circles contact-user-external-local Python
 Home-page: https://github.com/circles-zone/contact-user-external-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: database_mysql_local>=0.0.290
 Requires-Dist: logger-local>=0.0.135
 Requires-Dist: user-context-remote>=0.0.77
 Requires-Dist: user-external-local>=0.0.42
+Requires-Dist: internet-domain-local>=0.0.18
 
 PyPI Package for Circles contact-user-external-local Python
```

### Comparing `contact_user_external_local-0.0.7/contact_user_external_local/src/contact_user_external_local_constants.py` & `contact_user_external_local-0.0.8/contact_user_external_local/src/contact_user_external_local_constants.py`

 * *Files identical despite different names*

### Comparing `contact_user_external_local-0.0.7/contact_user_external_local.egg-info/PKG-INFO` & `contact_user_external_local-0.0.8/contact_user_external_local.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: contact-user-external-local
-Version: 0.0.7
+Version: 0.0.8
 Summary: PyPI Package for Circles contact-user-external-local Python
 Home-page: https://github.com/circles-zone/contact-user-external-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: database_mysql_local>=0.0.290
 Requires-Dist: logger-local>=0.0.135
 Requires-Dist: user-context-remote>=0.0.77
 Requires-Dist: user-external-local>=0.0.42
+Requires-Dist: internet-domain-local>=0.0.18
 
 PyPI Package for Circles contact-user-external-local Python
```

### Comparing `contact_user_external_local-0.0.7/setup.py` & `contact_user_external_local-0.0.8/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "contact-user-external-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.7',  # https://pypi.org/project/contact-user-external-local/
+    version='0.0.8',  # https://pypi.org/project/contact-user-external-local/
     author="Circles",
     author_email="info@circlez.ai",
     description="PyPI Package for Circles contact-user-external-local Python",
     long_description="PyPI Package for Circles contact-user-external-local Python",
     long_description_content_type='text/markdown',
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     package_dir={package_dir: f'{package_dir}/src'},
@@ -20,9 +20,10 @@
         "Operating System :: OS Independent",
     ],
     install_requires=[
         'database_mysql_local>=0.0.290',
         'logger-local>=0.0.135',
         'user-context-remote>=0.0.77',
         'user-external-local>=0.0.42',
+        'internet-domain-local>=0.0.18'
     ],
 )
```

