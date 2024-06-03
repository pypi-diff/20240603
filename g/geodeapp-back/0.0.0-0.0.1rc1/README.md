# Comparing `tmp/geodeapp_back-0.0.0.tar.gz` & `tmp/geodeapp_back-0.0.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geodeapp_back-0.0.0.tar", last modified: Fri May 17 13:11:28 2024, max compression
+gzip compressed data, was "geodeapp_back-0.0.1rc1.tar", last modified: Mon Jun  3 09:18:02 2024, max compression
```

## Comparing `geodeapp_back-0.0.0.tar` & `geodeapp_back-0.0.1rc1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:11:28.869981 geodeapp_back-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-17 13:11:16.000000 geodeapp_back-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-17 13:11:28.869981 geodeapp_back-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-17 13:11:16.000000 geodeapp_back-0.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-17 13:11:17.000000 geodeapp_back-0.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-05-17 13:11:16.000000 geodeapp_back-0.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 13:11:28.869981 geodeapp_back-0.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:11:28.865981 geodeapp_back-0.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:11:28.865981 geodeapp_back-0.0.0/src/geodeapp_back/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-17 13:11:16.000000 geodeapp_back-0.0.0/src/geodeapp_back/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-05-17 13:11:16.000000 geodeapp_back-0.0.0/src/geodeapp_back/app.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-17 13:11:16.000000 geodeapp_back-0.0.0/src/geodeapp_back/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:11:28.869981 geodeapp_back-0.0.0/src/geodeapp_back.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-17 13:11:28.000000 geodeapp_back-0.0.0/src/geodeapp_back.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-17 13:11:28.000000 geodeapp_back-0.0.0/src/geodeapp_back.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 13:11:28.000000 geodeapp_back-0.0.0/src/geodeapp_back.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-17 13:11:28.000000 geodeapp_back-0.0.0/src/geodeapp_back.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-17 13:11:28.000000 geodeapp_back-0.0.0/src/geodeapp_back.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-17 13:11:28.000000 geodeapp_back-0.0.0/src/geodeapp_back.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:11:28.865981 geodeapp_back-0.0.0/src/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 13:11:16.000000 geodeapp_back-0.0.0/src/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-17 13:11:16.000000 geodeapp_back-0.0.0/src/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-17 13:11:16.000000 geodeapp_back-0.0.0/src/tests/test_routes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:18:02.388767 geodeapp_back-0.0.1rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-06-03 09:17:51.000000 geodeapp_back-0.0.1rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-06-03 09:18:02.388767 geodeapp_back-0.0.1rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-06-03 09:17:51.000000 geodeapp_back-0.0.1rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-06-03 09:17:52.000000 geodeapp_back-0.0.1rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-06-03 09:17:51.000000 geodeapp_back-0.0.1rc1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 09:18:02.388767 geodeapp_back-0.0.1rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:18:02.384767 geodeapp_back-0.0.1rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:18:02.384767 geodeapp_back-0.0.1rc1/src/geodeapp_back/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-06-03 09:17:51.000000 geodeapp_back-0.0.1rc1/src/geodeapp_back/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-06-03 09:17:51.000000 geodeapp_back-0.0.1rc1/src/geodeapp_back/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-06-03 09:17:51.000000 geodeapp_back-0.0.1rc1/src/geodeapp_back/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:18:02.388767 geodeapp_back-0.0.1rc1/src/geodeapp_back.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-06-03 09:18:02.000000 geodeapp_back-0.0.1rc1/src/geodeapp_back.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-06-03 09:18:02.000000 geodeapp_back-0.0.1rc1/src/geodeapp_back.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 09:18:02.000000 geodeapp_back-0.0.1rc1/src/geodeapp_back.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-06-03 09:18:02.000000 geodeapp_back-0.0.1rc1/src/geodeapp_back.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-06-03 09:18:02.000000 geodeapp_back-0.0.1rc1/src/geodeapp_back.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-06-03 09:18:02.000000 geodeapp_back-0.0.1rc1/src/geodeapp_back.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:18:02.388767 geodeapp_back-0.0.1rc1/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:17:51.000000 geodeapp_back-0.0.1rc1/src/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-06-03 09:17:51.000000 geodeapp_back-0.0.1rc1/src/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-06-03 09:17:51.000000 geodeapp_back-0.0.1rc1/src/tests/test_routes.py
```

### Comparing `geodeapp_back-0.0.0/LICENSE` & `geodeapp_back-0.0.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `geodeapp_back-0.0.0/PKG-INFO` & `geodeapp_back-0.0.1rc1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,44 +1,43 @@
 Metadata-Version: 2.1
 Name: geodeapp_back
-Version: 0.0.0
+Version: 0.0.1rc1
 Author-email: Geode-solutions <team-web@geode-solutions.com>
 Project-URL: Homepage, https://github.com/Geode-solutions/geodeapp-back
 Project-URL: Bug Tracker, https://github.com/Geode-solutions/geodeapp-back/issues
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
-Requires-Dist: opengeodeweb-back==4.1.1
+Requires-Dist: opengeodeweb-back==4.2.1
 Requires-Dist: python-dotenv==1.0.1
-Requires-Dist: referencing==0.35.0
-Requires-Dist: rpds-py==0.18.0
-Requires-Dist: typing-extensions==4.11.0
-Requires-Dist: werkzeug==3.0.2
+Requires-Dist: referencing==0.35.1
+Requires-Dist: rpds-py==0.18.1
+Requires-Dist: werkzeug==3.0.3
 
 # GeodeApp-Back
```

### Comparing `geodeapp_back-0.0.0/pyproject.toml` & `geodeapp_back-0.0.1rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "geodeapp_back"
-version = "0.0.0"
+version = "0.0.1-rc.1"
 dynamic = ["dependencies"]
 authors = [
   { name="Geode-solutions", email="team-web@geode-solutions.com" },
 ]
 description = ""
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `geodeapp_back-0.0.0/requirements.txt` & `geodeapp_back-0.0.1rc1/requirements.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,140 +1,138 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    pip-compile
+#    pip-compile requirements.in
 #
 asgiref==3.8.1
     # via
     #   flask
     #   opengeodeweb-back
 attrs==23.2.0
     # via
     #   jsonschema
     #   opengeodeweb-back
     #   referencing
-blinker==1.8.1
+blinker==1.8.2
     # via
     #   flask
     #   opengeodeweb-back
 click==8.1.7
     # via
     #   flask
     #   opengeodeweb-back
 flask[async]==3.0.3
     # via
     #   flask-cors
     #   opengeodeweb-back
-flask-cors==4.0.0
+flask-cors==4.0.1
     # via opengeodeweb-back
-geode-background==7.9.8
+geode-background==7.12.0
     # via
     #   geode-explicit
     #   geode-implicit
     #   geode-simplex
     #   opengeodeweb-back
-geode-common==31.0.8
+geode-common==31.2.1
     # via
     #   geode-background
     #   geode-explicit
     #   geode-implicit
     #   geode-numerics
     #   geode-simplex
     #   geode-viewables
     #   opengeodeweb-back
-geode-conversion==5.2.8
+geode-conversion==5.4.1
     # via
     #   geode-explicit
     #   geode-implicit
     #   opengeodeweb-back
-geode-explicit==4.7.5
+geode-explicit==4.8.3
     # via
     #   geode-implicit
     #   opengeodeweb-back
-geode-implicit==2.8.6
+geode-implicit==2.8.7
     # via opengeodeweb-back
-geode-numerics==4.3.3
+geode-numerics==4.4.0
     # via
     #   geode-implicit
     #   geode-simplex
     #   opengeodeweb-back
-geode-simplex==6.7.4
+geode-simplex==6.8.3
     # via opengeodeweb-back
-geode-viewables==2.2.2
+geode-viewables==2.2.3
     # via opengeodeweb-back
 itsdangerous==2.2.0
     # via
     #   flask
     #   opengeodeweb-back
-jinja2==3.1.3
+jinja2==3.1.4
     # via
     #   flask
     #   opengeodeweb-back
-jsonschema==4.21.1
+jsonschema==4.22.0
     # via opengeodeweb-back
 jsonschema-specifications==2023.12.1
     # via
     #   jsonschema
     #   opengeodeweb-back
 markupsafe==2.1.5
     # via
     #   jinja2
     #   opengeodeweb-back
     #   werkzeug
-opengeode-core==14.19.2
+opengeode-core==14.21.3
     # via
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
     #   opengeodeweb-back
-opengeode-geosciences==7.6.4
+opengeode-geosciences==7.7.0
     # via
     #   geode-implicit
     #   geode-viewables
     #   opengeode-geosciencesio
     #   opengeodeweb-back
-opengeode-geosciencesio==4.7.6
+opengeode-geosciencesio==4.7.7
     # via
     #   geode-implicit
     #   opengeodeweb-back
-opengeode-inspector==5.1.3
+opengeode-inspector==5.1.4
     # via
     #   geode-explicit
     #   geode-implicit
     #   geode-simplex
     #   opengeodeweb-back
 opengeode-io==6.5.1
     # via
     #   geode-implicit
     #   geode-viewables
     #   opengeode-geosciencesio
     #   opengeodeweb-back
-opengeodeweb-back==4.1.1
+opengeodeweb-back==4.2.1
     # via -r requirements.in
 python-dotenv==1.0.1
     # via -r requirements.in
-referencing==0.35.0
+referencing==0.35.1
     # via
     #   jsonschema
     #   jsonschema-specifications
     #   opengeodeweb-back
-rpds-py==0.18.0
+rpds-py==0.18.1
     # via
     #   jsonschema
     #   opengeodeweb-back
     #   referencing
-typing-extensions==4.11.0
-    # via asgiref
-werkzeug==3.0.2
+werkzeug==3.0.3
     # via
     #   flask
     #   opengeodeweb-back
```

### Comparing `geodeapp_back-0.0.0/src/geodeapp_back/app.py` & `geodeapp_back-0.0.1rc1/src/geodeapp_back/app.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from opengeodeweb_back.routes import blueprint_routes
 
 from werkzeug.exceptions import HTTPException
 
 from werkzeug.exceptions import HTTPException
 
 from .config import *
+from opengeodeweb_back.geode_functions import handle_exception
 
 
 if os.path.isfile("./.env"):
     basedir = os.path.abspath(os.path.dirname(__file__))
     dotenv.load_dotenv(os.path.join(basedir, ".env"))
 
 """ Global config """
@@ -82,25 +83,16 @@
 
 if FLASK_DEBUG == False:
     geode_functions.set_interval(kill_task, SECONDS_BETWEEN_SHUTDOWNS)
 flask_cors.CORS(app, origins=ORIGINS)
 
 
 @app.errorhandler(HTTPException)
-def handle_exception(e):
-    response = e.get_response()
-    response.data = flask.json.dumps(
-        {
-            "code": e.code,
-            "name": e.name,
-            "description": e.description,
-        }
-    )
-    response.content_type = "application/json"
-    return response
+def errorhandler(e):
+    return handle_exception(e)
 
 
 @app.route("/geodeapp/createbackend", methods=["POST"])
 def create_backend():
     return flask.make_response({"ID": str("123456")}, 200)
```

### Comparing `geodeapp_back-0.0.0/src/geodeapp_back/config.py` & `geodeapp_back-0.0.1rc1/src/geodeapp_back/config.py`

 * *Files identical despite different names*

### Comparing `geodeapp_back-0.0.0/src/geodeapp_back.egg-info/PKG-INFO` & `geodeapp_back-0.0.1rc1/src/geodeapp_back.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,44 +1,43 @@
 Metadata-Version: 2.1
 Name: geodeapp_back
-Version: 0.0.0
+Version: 0.0.1rc1
 Author-email: Geode-solutions <team-web@geode-solutions.com>
 Project-URL: Homepage, https://github.com/Geode-solutions/geodeapp-back
 Project-URL: Bug Tracker, https://github.com/Geode-solutions/geodeapp-back/issues
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
-Requires-Dist: opengeodeweb-back==4.1.1
+Requires-Dist: opengeodeweb-back==4.2.1
 Requires-Dist: python-dotenv==1.0.1
-Requires-Dist: referencing==0.35.0
-Requires-Dist: rpds-py==0.18.0
-Requires-Dist: typing-extensions==4.11.0
-Requires-Dist: werkzeug==3.0.2
+Requires-Dist: referencing==0.35.1
+Requires-Dist: rpds-py==0.18.1
+Requires-Dist: werkzeug==3.0.3
 
 # GeodeApp-Back
```

