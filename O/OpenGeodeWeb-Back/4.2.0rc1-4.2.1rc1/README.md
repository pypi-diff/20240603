# Comparing `tmp/opengeodeweb_back-4.2.0rc1.tar.gz` & `tmp/opengeodeweb_back-4.2.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opengeodeweb_back-4.2.0rc1.tar", last modified: Mon May 27 10:11:09 2024, max compression
+gzip compressed data, was "opengeodeweb_back-4.2.1rc1.tar", last modified: Mon Jun  3 08:57:12 2024, max compression
```

## Comparing `opengeodeweb_back-4.2.0rc1.tar` & `opengeodeweb_back-4.2.1rc1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:11:09.553610 opengeodeweb_back-4.2.0rc1/
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-27 10:10:53.000000 opengeodeweb_back-4.2.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-27 10:11:09.553610 opengeodeweb_back-4.2.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-27 10:10:53.000000 opengeodeweb_back-4.2.0rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-27 10:11:00.000000 opengeodeweb_back-4.2.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-27 10:10:53.000000 opengeodeweb_back-4.2.0rc1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 10:11:09.553610 opengeodeweb_back-4.2.0rc1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:11:09.549610 opengeodeweb_back-4.2.0rc1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:11:09.553610 opengeodeweb_back-4.2.0rc1/src/OpenGeodeWeb_Back.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-27 10:11:09.000000 opengeodeweb_back-4.2.0rc1/src/OpenGeodeWeb_Back.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-27 10:11:09.000000 opengeodeweb_back-4.2.0rc1/src/OpenGeodeWeb_Back.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 10:11:09.000000 opengeodeweb_back-4.2.0rc1/src/OpenGeodeWeb_Back.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-27 10:11:09.000000 opengeodeweb_back-4.2.0rc1/src/OpenGeodeWeb_Back.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 10:11:09.000000 opengeodeweb_back-4.2.0rc1/src/OpenGeodeWeb_Back.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:11:09.553610 opengeodeweb_back-4.2.0rc1/src/opengeodeweb_back/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 10:10:53.000000 opengeodeweb_back-4.2.0rc1/src/opengeodeweb_back/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11637 2024-05-27 10:10:53.000000 opengeodeweb_back-4.2.0rc1/src/opengeodeweb_back/geode_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    20286 2024-05-27 10:10:53.000000 opengeodeweb_back-4.2.0rc1/src/opengeodeweb_back/geode_objects.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:11:09.553610 opengeodeweb_back-4.2.0rc1/src/opengeodeweb_back/routes/
--rw-r--r--   0 runner    (1001) docker     (127)     6082 2024-05-27 10:10:53.000000 opengeodeweb_back-4.2.0rc1/src/opengeodeweb_back/routes/blueprint_routes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:11:09.553610 opengeodeweb_back-4.2.0rc1/src/opengeodeweb_back/routes/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-27 10:10:53.000000 opengeodeweb_back-4.2.0rc1/src/opengeodeweb_back/routes/schemas/allowed_files.json
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-27 10:10:53.000000 opengeodeweb_back-4.2.0rc1/src/opengeodeweb_back/routes/schemas/allowed_objects.json
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-27 10:10:53.000000 opengeodeweb_back-4.2.0rc1/src/opengeodeweb_back/routes/schemas/geode_objects_and_output_extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-27 10:10:53.000000 opengeodeweb_back-4.2.0rc1/src/opengeodeweb_back/routes/schemas/geographic_coordinate_systems.json
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-27 10:10:53.000000 opengeodeweb_back-4.2.0rc1/src/opengeodeweb_back/routes/schemas/inspect_file.json
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-27 10:10:53.000000 opengeodeweb_back-4.2.0rc1/src/opengeodeweb_back/routes/schemas/missing_files.json
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-27 10:10:53.000000 opengeodeweb_back-4.2.0rc1/src/opengeodeweb_back/routes/schemas/upload_file.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:11:09.553610 opengeodeweb_back-4.2.0rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    14659 2024-05-27 10:10:53.000000 opengeodeweb_back-4.2.0rc1/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-05-27 10:10:53.000000 opengeodeweb_back-4.2.0rc1/tests/test_routes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:57:12.323277 opengeodeweb_back-4.2.1rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-06-03 08:56:55.000000 opengeodeweb_back-4.2.1rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-06-03 08:57:12.323277 opengeodeweb_back-4.2.1rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-06-03 08:56:55.000000 opengeodeweb_back-4.2.1rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-06-03 08:57:02.000000 opengeodeweb_back-4.2.1rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-06-03 08:56:55.000000 opengeodeweb_back-4.2.1rc1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 08:57:12.323277 opengeodeweb_back-4.2.1rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:57:12.319276 opengeodeweb_back-4.2.1rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:57:12.323277 opengeodeweb_back-4.2.1rc1/src/OpenGeodeWeb_Back.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-06-03 08:57:12.000000 opengeodeweb_back-4.2.1rc1/src/OpenGeodeWeb_Back.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-06-03 08:57:12.000000 opengeodeweb_back-4.2.1rc1/src/OpenGeodeWeb_Back.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 08:57:12.000000 opengeodeweb_back-4.2.1rc1/src/OpenGeodeWeb_Back.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-06-03 08:57:12.000000 opengeodeweb_back-4.2.1rc1/src/OpenGeodeWeb_Back.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-06-03 08:57:12.000000 opengeodeweb_back-4.2.1rc1/src/OpenGeodeWeb_Back.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:57:12.319276 opengeodeweb_back-4.2.1rc1/src/opengeodeweb_back/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 08:56:55.000000 opengeodeweb_back-4.2.1rc1/src/opengeodeweb_back/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11637 2024-06-03 08:56:55.000000 opengeodeweb_back-4.2.1rc1/src/opengeodeweb_back/geode_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20290 2024-06-03 08:56:55.000000 opengeodeweb_back-4.2.1rc1/src/opengeodeweb_back/geode_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:57:12.319276 opengeodeweb_back-4.2.1rc1/src/opengeodeweb_back/routes/
+-rw-r--r--   0 runner    (1001) docker     (127)     6082 2024-06-03 08:56:55.000000 opengeodeweb_back-4.2.1rc1/src/opengeodeweb_back/routes/blueprint_routes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:57:12.323277 opengeodeweb_back-4.2.1rc1/src/opengeodeweb_back/routes/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-06-03 08:56:55.000000 opengeodeweb_back-4.2.1rc1/src/opengeodeweb_back/routes/schemas/allowed_files.json
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-06-03 08:56:55.000000 opengeodeweb_back-4.2.1rc1/src/opengeodeweb_back/routes/schemas/allowed_objects.json
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-06-03 08:56:55.000000 opengeodeweb_back-4.2.1rc1/src/opengeodeweb_back/routes/schemas/geode_objects_and_output_extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-06-03 08:56:55.000000 opengeodeweb_back-4.2.1rc1/src/opengeodeweb_back/routes/schemas/geographic_coordinate_systems.json
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-06-03 08:56:55.000000 opengeodeweb_back-4.2.1rc1/src/opengeodeweb_back/routes/schemas/inspect_file.json
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-06-03 08:56:55.000000 opengeodeweb_back-4.2.1rc1/src/opengeodeweb_back/routes/schemas/missing_files.json
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-06-03 08:56:55.000000 opengeodeweb_back-4.2.1rc1/src/opengeodeweb_back/routes/schemas/upload_file.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 08:57:12.323277 opengeodeweb_back-4.2.1rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    14659 2024-06-03 08:56:55.000000 opengeodeweb_back-4.2.1rc1/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-06-03 08:56:55.000000 opengeodeweb_back-4.2.1rc1/tests/test_routes.py
```

### Comparing `opengeodeweb_back-4.2.0rc1/LICENSE` & `opengeodeweb_back-4.2.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `opengeodeweb_back-4.2.0rc1/PKG-INFO` & `opengeodeweb_back-4.2.1rc1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 Metadata-Version: 2.1
 Name: OpenGeodeWeb-Back
-Version: 4.2.0rc1
+Version: 4.2.1rc1
 Summary: OpenGeodeWeb-Back is an open source framework that proposes handy python functions and wrappers for the OpenGeode ecosystem
 Author-email: Geode-solutions <team-web@geode-solutions.com>
 Project-URL: Homepage, https://github.com/Geode-solutions/OpenGeodeWeb-Back
 Project-URL: Bug Tracker, https://github.com/Geode-solutions/OpenGeodeWeb-Back/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: asgiref==3.8.1
 Requires-Dist: attrs==23.2.0
-Requires-Dist: blinker==1.8.1
+Requires-Dist: blinker==1.8.2
 Requires-Dist: click==8.1.7
 Requires-Dist: flask[async]==3.0.3
-Requires-Dist: flask-cors==4.0.0
-Requires-Dist: geode-background==7.9.8
-Requires-Dist: geode-common==31.0.8
-Requires-Dist: geode-conversion==5.2.8
-Requires-Dist: geode-explicit==4.7.5
-Requires-Dist: geode-implicit==2.8.6
-Requires-Dist: geode-numerics==4.3.3
-Requires-Dist: geode-simplex==6.7.4
-Requires-Dist: geode-viewables==2.2.2
+Requires-Dist: flask-cors==4.0.1
+Requires-Dist: geode-background==7.12.0
+Requires-Dist: geode-common==31.2.1
+Requires-Dist: geode-conversion==5.4.1
+Requires-Dist: geode-explicit==4.8.3
+Requires-Dist: geode-implicit==2.8.7
+Requires-Dist: geode-numerics==4.4.0
+Requires-Dist: geode-simplex==6.8.3
+Requires-Dist: geode-viewables==2.2.3
 Requires-Dist: itsdangerous==2.2.0
-Requires-Dist: jinja2==3.1.3
-Requires-Dist: jsonschema==4.21.1
+Requires-Dist: jinja2==3.1.4
+Requires-Dist: jsonschema==4.22.0
 Requires-Dist: jsonschema-specifications==2023.12.1
 Requires-Dist: markupsafe==2.1.5
-Requires-Dist: opengeode-core==14.19.2
-Requires-Dist: opengeode-geosciences==7.6.4
-Requires-Dist: opengeode-geosciencesio==4.7.6
-Requires-Dist: opengeode-inspector==5.1.3
+Requires-Dist: opengeode-core==14.21.3
+Requires-Dist: opengeode-geosciences==7.7.0
+Requires-Dist: opengeode-geosciencesio==4.7.7
+Requires-Dist: opengeode-inspector==5.1.4
 Requires-Dist: opengeode-io==6.5.1
-Requires-Dist: referencing==0.35.0
-Requires-Dist: rpds-py==0.18.0
-Requires-Dist: typing-extensions==4.12.0
-Requires-Dist: werkzeug==3.0.2
+Requires-Dist: referencing==0.35.1
+Requires-Dist: rpds-py==0.18.1
+Requires-Dist: werkzeug==3.0.3
 
 <h1 align="center">OpenGeodeWeb-Back<sup><i>by Geode-solutions</i></sup></h1>
 <h3 align="center">OpenSource Python framework based on OpenGeode</h3>
 
 <p align="center">
   <img src="https://github.com/Geode-solutions/OpenGeodeWeb-Back/workflows/CI/badge.svg" alt="Build Status">
   <img src="https://github.com/Geode-solutions/OpenGeodeWeb-Back/workflows/CD/badge.svg" alt="Deploy Status">
```

### Comparing `opengeodeweb_back-4.2.0rc1/README.md` & `opengeodeweb_back-4.2.1rc1/README.md`

 * *Files identical despite different names*

### Comparing `opengeodeweb_back-4.2.0rc1/pyproject.toml` & `opengeodeweb_back-4.2.1rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "OpenGeodeWeb-Back"
-version = "4.2.0-rc.1"
+version = "4.2.1-rc.1"
 dynamic = ["dependencies"]
 authors = [
   { name="Geode-solutions", email="team-web@geode-solutions.com" },
 ]
 description = "OpenGeodeWeb-Back is an open source framework that proposes handy python functions and wrappers for the OpenGeode ecosystem"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `opengeodeweb_back-4.2.0rc1/requirements.txt` & `opengeodeweb_back-4.2.1rc1/requirements.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,118 +1,116 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
 #    pip-compile requirements.in
 #
 asgiref==3.8.1
     # via flask
 attrs==23.2.0
     # via
     #   jsonschema
     #   referencing
-blinker==1.8.1
+blinker==1.8.2
     # via flask
 click==8.1.7
     # via flask
 flask[async]==3.0.3
     # via
     #   -r requirements.in
     #   flask-cors
-flask-cors==4.0.0
+flask-cors==4.0.1
     # via -r requirements.in
-geode-background==7.9.8
+geode-background==7.12.0
     # via
     #   geode-explicit
     #   geode-implicit
     #   geode-simplex
-geode-common==31.0.8
+geode-common==31.2.1
     # via
     #   -r requirements.in
     #   geode-background
     #   geode-explicit
     #   geode-implicit
     #   geode-numerics
     #   geode-simplex
     #   geode-viewables
-geode-conversion==5.2.8
+geode-conversion==5.4.1
     # via
     #   geode-explicit
     #   geode-implicit
-geode-explicit==4.7.5
+geode-explicit==4.8.3
     # via
     #   -r requirements.in
     #   geode-implicit
-geode-implicit==2.8.6
+geode-implicit==2.8.7
     # via -r requirements.in
-geode-numerics==4.3.3
+geode-numerics==4.4.0
     # via
     #   -r requirements.in
     #   geode-implicit
     #   geode-simplex
-geode-simplex==6.7.4
+geode-simplex==6.8.3
     # via -r requirements.in
-geode-viewables==2.2.2
+geode-viewables==2.2.3
     # via -r requirements.in
 itsdangerous==2.2.0
     # via flask
-jinja2==3.1.3
+jinja2==3.1.4
     # via flask
-jsonschema==4.21.1
+jsonschema==4.22.0
     # via -r requirements.in
 jsonschema-specifications==2023.12.1
     # via jsonschema
 markupsafe==2.1.5
     # via
     #   jinja2
     #   werkzeug
-opengeode-core==14.19.2
+opengeode-core==14.21.3
     # via
     #   -r requirements.in
     #   geode-background
     #   geode-common
     #   geode-conversion
     #   geode-explicit
     #   geode-implicit
     #   geode-numerics
     #   geode-simplex
     #   geode-viewables
     #   opengeode-geosciences
     #   opengeode-geosciencesio
     #   opengeode-inspector
     #   opengeode-io
-opengeode-geosciences==7.6.4
+opengeode-geosciences==7.7.0
     # via
     #   -r requirements.in
     #   geode-implicit
     #   geode-viewables
     #   opengeode-geosciencesio
-opengeode-geosciencesio==4.7.6
+opengeode-geosciencesio==4.7.7
     # via
     #   -r requirements.in
     #   geode-implicit
-opengeode-inspector==5.1.3
+opengeode-inspector==5.1.4
     # via
     #   -r requirements.in
     #   geode-explicit
     #   geode-implicit
     #   geode-simplex
 opengeode-io==6.5.1
     # via
     #   -r requirements.in
     #   geode-implicit
     #   geode-viewables
     #   opengeode-geosciencesio
-referencing==0.35.0
+referencing==0.35.1
     # via
     #   jsonschema
     #   jsonschema-specifications
-rpds-py==0.18.0
+rpds-py==0.18.1
     # via
     #   jsonschema
     #   referencing
-typing-extensions==4.12.0
-    # via asgiref
-werkzeug==3.0.2
+werkzeug==3.0.3
     # via
     #   -r requirements.in
     #   flask
```

### Comparing `opengeodeweb_back-4.2.0rc1/src/OpenGeodeWeb_Back.egg-info/PKG-INFO` & `opengeodeweb_back-4.2.1rc1/src/OpenGeodeWeb_Back.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 Metadata-Version: 2.1
 Name: OpenGeodeWeb-Back
-Version: 4.2.0rc1
+Version: 4.2.1rc1
 Summary: OpenGeodeWeb-Back is an open source framework that proposes handy python functions and wrappers for the OpenGeode ecosystem
 Author-email: Geode-solutions <team-web@geode-solutions.com>
 Project-URL: Homepage, https://github.com/Geode-solutions/OpenGeodeWeb-Back
 Project-URL: Bug Tracker, https://github.com/Geode-solutions/OpenGeodeWeb-Back/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: asgiref==3.8.1
 Requires-Dist: attrs==23.2.0
-Requires-Dist: blinker==1.8.1
+Requires-Dist: blinker==1.8.2
 Requires-Dist: click==8.1.7
 Requires-Dist: flask[async]==3.0.3
-Requires-Dist: flask-cors==4.0.0
-Requires-Dist: geode-background==7.9.8
-Requires-Dist: geode-common==31.0.8
-Requires-Dist: geode-conversion==5.2.8
-Requires-Dist: geode-explicit==4.7.5
-Requires-Dist: geode-implicit==2.8.6
-Requires-Dist: geode-numerics==4.3.3
-Requires-Dist: geode-simplex==6.7.4
-Requires-Dist: geode-viewables==2.2.2
+Requires-Dist: flask-cors==4.0.1
+Requires-Dist: geode-background==7.12.0
+Requires-Dist: geode-common==31.2.1
+Requires-Dist: geode-conversion==5.4.1
+Requires-Dist: geode-explicit==4.8.3
+Requires-Dist: geode-implicit==2.8.7
+Requires-Dist: geode-numerics==4.4.0
+Requires-Dist: geode-simplex==6.8.3
+Requires-Dist: geode-viewables==2.2.3
 Requires-Dist: itsdangerous==2.2.0
-Requires-Dist: jinja2==3.1.3
-Requires-Dist: jsonschema==4.21.1
+Requires-Dist: jinja2==3.1.4
+Requires-Dist: jsonschema==4.22.0
 Requires-Dist: jsonschema-specifications==2023.12.1
 Requires-Dist: markupsafe==2.1.5
-Requires-Dist: opengeode-core==14.19.2
-Requires-Dist: opengeode-geosciences==7.6.4
-Requires-Dist: opengeode-geosciencesio==4.7.6
-Requires-Dist: opengeode-inspector==5.1.3
+Requires-Dist: opengeode-core==14.21.3
+Requires-Dist: opengeode-geosciences==7.7.0
+Requires-Dist: opengeode-geosciencesio==4.7.7
+Requires-Dist: opengeode-inspector==5.1.4
 Requires-Dist: opengeode-io==6.5.1
-Requires-Dist: referencing==0.35.0
-Requires-Dist: rpds-py==0.18.0
-Requires-Dist: typing-extensions==4.12.0
-Requires-Dist: werkzeug==3.0.2
+Requires-Dist: referencing==0.35.1
+Requires-Dist: rpds-py==0.18.1
+Requires-Dist: werkzeug==3.0.3
 
 <h1 align="center">OpenGeodeWeb-Back<sup><i>by Geode-solutions</i></sup></h1>
 <h3 align="center">OpenSource Python framework based on OpenGeode</h3>
 
 <p align="center">
   <img src="https://github.com/Geode-solutions/OpenGeodeWeb-Back/workflows/CI/badge.svg" alt="Build Status">
   <img src="https://github.com/Geode-solutions/OpenGeodeWeb-Back/workflows/CD/badge.svg" alt="Deploy Status">
```

### Comparing `opengeodeweb_back-4.2.0rc1/src/OpenGeodeWeb_Back.egg-info/SOURCES.txt` & `opengeodeweb_back-4.2.1rc1/src/OpenGeodeWeb_Back.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opengeodeweb_back-4.2.0rc1/src/opengeodeweb_back/geode_functions.py` & `opengeodeweb_back-4.2.1rc1/src/opengeodeweb_back/geode_functions.py`

 * *Files identical despite different names*

### Comparing `opengeodeweb_back-4.2.0rc1/src/opengeodeweb_back/geode_objects.py` & `opengeodeweb_back-4.2.1rc1/src/opengeodeweb_back/geode_objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
                 "convert": og_gs.convert_edged_curve_coordinate_reference_system2D,
                 "create": og.create_edged_curve_coordinate_system2D,
             },
             "is_model": False,
             "is_3D": False,
             "is_viewable": True,
             "save_viewable": g_v.save_viewable_edged_curve2D,
-            "inspector": og_inspector.inspect_edgedcurve2D,
+            "inspector": og_inspector.inspect_edged_curve2D,
         },
         "EdgedCurve3D": {
             "input_factory": og.EdgedCurveInputFactory3D,
             "output_factory": og.EdgedCurveOutputFactory3D,
             "missing_files": og.check_edged_curve_missing_files3D,
             "is_loadable": og.is_edged_curve_loadable3D,
             "load": og.load_edged_curve3D,
@@ -83,15 +83,15 @@
                 "convert": og_gs.convert_edged_curve_coordinate_reference_system3D,
                 "create": og.create_edged_curve_coordinate_system3D,
             },
             "is_model": False,
             "is_3D": True,
             "is_viewable": True,
             "save_viewable": g_v.save_viewable_edged_curve3D,
-            "inspector": og_inspector.inspect_edgedcurve3D,
+            "inspector": og_inspector.inspect_edged_curve3D,
         },
         "Graph": {
             "input_factory": og.GraphInputFactory,
             "output_factory": og.GraphOutputFactory,
             "missing_files": og.check_graph_missing_files,
             "is_loadable": og.is_graph_loadable,
             "load": og.load_graph,
@@ -162,15 +162,15 @@
                 "convert": og_gs.convert_point_set_coordinate_reference_system2D,
                 "create": og.create_point_set_coordinate_system2D,
             },
             "is_model": False,
             "is_3D": False,
             "is_viewable": True,
             "save_viewable": g_v.save_viewable_point_set2D,
-            "inspector": og_inspector.inspect_pointset2D,
+            "inspector": og_inspector.inspect_point_set2D,
         },
         "PointSet3D": {
             "input_factory": og.PointSetInputFactory3D,
             "output_factory": og.PointSetOutputFactory3D,
             "missing_files": og.check_point_set_missing_files3D,
             "is_loadable": og.is_point_set_loadable3D,
             "load": og.load_point_set3D,
@@ -182,15 +182,15 @@
                 "convert": og_gs.convert_point_set_coordinate_reference_system3D,
                 "create": og.create_point_set_coordinate_system3D,
             },
             "is_model": False,
             "is_3D": True,
             "is_viewable": True,
             "save_viewable": g_v.save_viewable_point_set3D,
-            "inspector": og_inspector.inspect_pointset3D,
+            "inspector": og_inspector.inspect_point_set3D,
         },
         "PolygonalSurface2D": {
             "input_factory": og.PolygonalSurfaceInputFactory2D,
             "output_factory": og.PolygonalSurfaceOutputFactory2D,
             "missing_files": og.check_polygonal_surface_missing_files2D,
             "is_loadable": og.is_polygonal_surface_loadable2D,
             "load": og.load_polygonal_surface2D,
```

### Comparing `opengeodeweb_back-4.2.0rc1/src/opengeodeweb_back/routes/blueprint_routes.py` & `opengeodeweb_back-4.2.1rc1/src/opengeodeweb_back/routes/blueprint_routes.py`

 * *Files identical despite different names*

### Comparing `opengeodeweb_back-4.2.0rc1/tests/test_functions.py` & `opengeodeweb_back-4.2.1rc1/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `opengeodeweb_back-4.2.0rc1/tests/test_routes.py` & `opengeodeweb_back-4.2.1rc1/tests/test_routes.py`

 * *Files identical despite different names*

