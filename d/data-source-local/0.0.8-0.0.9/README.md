# Comparing `tmp/data_source_local-0.0.8.tar.gz` & `tmp/data_source_local-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_source_local-0.0.8.tar", last modified: Tue May 21 21:26:44 2024, max compression
+gzip compressed data, was "data_source_local-0.0.9.tar", last modified: Mon Jun  3 14:20:42 2024, max compression
```

## Comparing `data_source_local-0.0.8.tar` & `data_source_local-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:26:44.295701 data_source_local-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-21 21:26:44.295701 data_source_local-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-21 21:26:27.000000 data_source_local-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:26:44.291701 data_source_local-0.0.8/data_source_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:26:44.291701 data_source_local-0.0.8/data_source_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 21:26:27.000000 data_source_local-0.0.8/data_source_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10920 2024-05-21 21:26:27.000000 data_source_local-0.0.8/data_source_local/src/data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-21 21:26:27.000000 data_source_local-0.0.8/data_source_local/src/data_source_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-21 21:26:27.000000 data_source_local-0.0.8/data_source_local/src/data_source_enum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:26:44.295701 data_source_local-0.0.8/data_source_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-21 21:26:44.000000 data_source_local-0.0.8/data_source_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-21 21:26:44.000000 data_source_local-0.0.8/data_source_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 21:26:44.000000 data_source_local-0.0.8/data_source_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-21 21:26:44.000000 data_source_local-0.0.8/data_source_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-21 21:26:44.000000 data_source_local-0.0.8/data_source_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-21 21:26:27.000000 data_source_local-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 21:26:44.295701 data_source_local-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-21 21:26:27.000000 data_source_local-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:20:42.114865 data_source_local-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-06-03 14:20:42.114865 data_source_local-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-06-03 14:20:02.000000 data_source_local-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:20:42.110865 data_source_local-0.0.9/data_source_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:20:42.114865 data_source_local-0.0.9/data_source_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:20:02.000000 data_source_local-0.0.9/data_source_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10962 2024-06-03 14:20:02.000000 data_source_local-0.0.9/data_source_local/src/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-06-03 14:20:02.000000 data_source_local-0.0.9/data_source_local/src/data_source_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-06-03 14:20:02.000000 data_source_local-0.0.9/data_source_local/src/data_source_enum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:20:42.114865 data_source_local-0.0.9/data_source_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-06-03 14:20:42.000000 data_source_local-0.0.9/data_source_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-06-03 14:20:42.000000 data_source_local-0.0.9/data_source_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 14:20:42.000000 data_source_local-0.0.9/data_source_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-06-03 14:20:42.000000 data_source_local-0.0.9/data_source_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-06-03 14:20:42.000000 data_source_local-0.0.9/data_source_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-06-03 14:20:11.000000 data_source_local-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 14:20:42.114865 data_source_local-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-06-03 14:20:02.000000 data_source_local-0.0.9/setup.py
```

### Comparing `data_source_local-0.0.8/README.md` & `data_source_local-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `data_source_local-0.0.8/data_source_local/src/data_source.py` & `data_source_local-0.0.9/data_source_local/src/data_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,14 +180,15 @@
             'notes': {"field_name": 'Notes'},
             'email1': {"field_name": 'Email', "index": 1},
             'email2': {"field_name": 'Email', "index": 2},
             'email3': {"field_name": 'Email', "index": 3},
             'website1': {"field_name": 'Website', "index": 1},
             'website2': {"field_name": 'Website', "index": 2},
             'website3': {"field_name": 'Website', "index": 3},
+            'url': {"field_name": 'URL'},
             'display_as': {"field_name": 'Display As'},
             'job_title': {"field_name": 'Job Title'},
             'organization': {"field_name": 'Organization/Company'},
             'department': {"field_name": 'Department'},
             'handle': {"field_name": 'LinkedIn Profile ID'},
             'address1_street': {"field_name": 'Home Street'},
             'address1_city': {"field_name": 'City'},
```

### Comparing `data_source_local-0.0.8/setup.py` & `data_source_local-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "data-source-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/data-source-local
-    version='0.0.8',
+    version='0.0.9',
     author="Circles",
     author_email="info@circles.ai",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description=PACKAGE_NAME,
```

