# Comparing `tmp/neno-0.0.11.tar.gz` & `tmp/neno-0.0.12.tar.gz`

## Comparing `neno-0.0.11.tar` & `neno-0.0.12.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 neno-0.0.11/Dockerfile
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 neno-0.0.11/src/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neno-0.0.11/src/neno/__init__.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 neno-0.0.11/src/neno/__main__.py
--rw-r--r--   0        0        0     6468 2020-02-02 00:00:00.000000 neno-0.0.11/src/neno/app.py
--rw-r--r--   0        0        0     9435 2020-02-02 00:00:00.000000 neno-0.0.11/src/neno/client.py
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 neno-0.0.11/src/neno/config.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 neno-0.0.11/src/neno/config.yaml
--rw-r--r--   0        0        0     8806 2020-02-02 00:00:00.000000 neno-0.0.11/src/neno/config_backends.py
--rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 neno-0.0.11/src/neno/models.py
--rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 neno-0.0.11/src/neno/requirements.txt
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 neno-0.0.11/src/neno/runner.py
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 neno-0.0.11/src/neno/server.py
--rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 neno-0.0.11/src/neno/storage_backends.py
--rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 neno-0.0.11/src/neno/util.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 neno-0.0.11/src/neno/example-endpoint/manifest.json
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 neno-0.0.11/src/neno/example-endpoint/template.txt
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 neno-0.0.11/src/neno/example-endpoint/test-notebook.ipynb
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 neno-0.0.11/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 neno-0.0.11/LICENSE
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 neno-0.0.11/README.md
--rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 neno-0.0.11/pyproject.toml
--rw-r--r--   0        0        0     6756 2020-02-02 00:00:00.000000 neno-0.0.11/PKG-INFO
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 neno-0.0.12/Dockerfile
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 neno-0.0.12/src/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neno-0.0.12/src/neno/__init__.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 neno-0.0.12/src/neno/__main__.py
+-rw-r--r--   0        0        0     6712 2020-02-02 00:00:00.000000 neno-0.0.12/src/neno/app.py
+-rw-r--r--   0        0        0    10476 2020-02-02 00:00:00.000000 neno-0.0.12/src/neno/client.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 neno-0.0.12/src/neno/config.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 neno-0.0.12/src/neno/config.yaml
+-rw-r--r--   0        0        0     8806 2020-02-02 00:00:00.000000 neno-0.0.12/src/neno/config_backends.py
+-rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 neno-0.0.12/src/neno/models.py
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 neno-0.0.12/src/neno/requirements.txt
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 neno-0.0.12/src/neno/runner.py
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 neno-0.0.12/src/neno/server.py
+-rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 neno-0.0.12/src/neno/storage_backends.py
+-rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 neno-0.0.12/src/neno/util.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 neno-0.0.12/src/neno/example-endpoint/manifest.json
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 neno-0.0.12/src/neno/example-endpoint/template.txt
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 neno-0.0.12/src/neno/example-endpoint/test-notebook.ipynb
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 neno-0.0.12/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 neno-0.0.12/LICENSE
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 neno-0.0.12/README.md
+-rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 neno-0.0.12/pyproject.toml
+-rw-r--r--   0        0        0     6756 2020-02-02 00:00:00.000000 neno-0.0.12/PKG-INFO
```

### Comparing `neno-0.0.11/src/neno/app.py` & `neno-0.0.12/src/neno/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import os, json, time, shutil, traceback, subprocess
+import os, json, time, shutil, traceback, subprocess, importlib.metadata
 
 def create_flask_app(config_file):
   from flask import Flask, request, jsonify, Response, request, send_file
   from .runner import run_notebook
   from flask import Flask
   from .models import EndpointSchema, NotaConfigSchema
   from .storage_backends import FsBackend
@@ -76,15 +76,15 @@
       if endpoint['content_type'] == 'application/json':
         resp = { 'status': 'success' if error_message is None else 'error', 'run_id': id }
         if output is not None:
           resp['response'] = json.loads(output)
         elif error_message is not None:
           resp['message'] = error_message
         return jsonify(resp), 200 if error_message is None else 500
-      return Response(output if output else error_message, mimetype=endpoint['content_type'])
+      return Response(output if output else error_message, mimetype=endpoint['content_type'], status=200 if error_message is None else 500)
     except Exception as e:
       traceback.print_exc()
       return jsonify({'status': 'error', 'message': str(e), 'run_id': id}), 500
 
   # Endpoint for posting new endpoints
   @app.route('/manage/endpoints', methods=['POST'])
   def add_endpoint():
@@ -140,8 +140,12 @@
   @app.route('/manage/kernels', methods=['GET'])
   def list_kernels():
     # run jupyter kernelspec list
     command = ['jupyter', 'kernelspec', 'list', '--json']
     kernelspecs = json.loads(subprocess.run(command, stdout=subprocess.PIPE).stdout.decode('utf-8'))
     return jsonify(kernelspecs)
   
+  @app.route('/manage/version', methods=['GET'])
+  def get_version():
+    return jsonify({'version': importlib.metadata.version('neno') or 'unknown (not installed via pip)'})
+  
   return app, config
```

### Comparing `neno-0.0.11/src/neno/client.py` & `neno-0.0.12/src/neno/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,17 +43,17 @@
 
 @cliApp.command(short_help="Start neno server.",
                 help="""Start the neno server and begin serving endpoints. Be sure to first install the server dependencies by running `pip install \"neno[server]\"`.
                 This command will look for a config.yaml file in the current directory and use it to configure the server.
                 The server will listen on 0.0.0.0:<port>, where port is 5000 by default.
                 """, name="serve")
 def serve(config_file: Annotated[str, typer.Option(help="The path to the config file to use. If not specified, will look for a config.yaml in the current folder.")] = "config.yaml"):
-  app, config = create_flask_app(config_file)
-  print(f"Starting server on {config['host']}:{config['port']}...")
   try:
+    app, config = create_flask_app(config_file)
+    print(f"Starting server on {config['host']}:{config['port']}...")
     gunicorn_run(app, port=config['port'])
   except ImportError as e:
     print("Failed to start server. Make sure you have installed neno[server]. You can do so by running `pip install \"neno[server]\"`.")
     print(f"Raw error: {e}")
 
 @getApp.command(short_help="List installed endpoints.")
 def endpoints(show_curl: Annotated[bool, typer.Option(help="Generate a curl command")] = False):
@@ -203,7 +203,33 @@
     response = requests.delete(f"{get_neno_server_url()}/manage/endpoints/" + name)
   except ConnectionError as e:
     print_connection_error(e)
     return
   if response.status_code < 200 or response.status_code >= 400:
     raise Exception(f"Failed to delete endpoint: {response.status_code} {response.text}")
   print(f"Deleted endpoint {name}.")
+
+versionApp = typer.Typer()
+cliApp.add_typer(versionApp, name="version", short_help="Get version information about the neno server or client.")
+
+@versionApp.command(name="client", short_help="Get the version of the neno client.")
+def version_client():
+  import importlib.metadata
+  print(f"Neno client version {importlib.metadata.version('neno') or 'unknown (not installed with pip)'}")
+
+@versionApp.command(name="server", short_help="Get the version of the neno server.")
+def version_server():
+  no_version = "Could not get the server version. The server is either running a pre-0.0.12 version of neno or is not running neno at all."
+  response = None
+  try:
+    response = requests.get(f"{get_neno_server_url()}/manage/version")
+    try:
+      response = response.json()
+      if 'version' in response.keys():
+        print(f"Neno server version {response.get('version')}")
+      else:
+        print(no_version)
+    except Exception as e:
+      print(no_version)
+  except ConnectionError as e:
+    print_connection_error(e)
+    return
```

### Comparing `neno-0.0.11/src/neno/config_backends.py` & `neno-0.0.12/src/neno/config_backends.py`

 * *Files identical despite different names*

### Comparing `neno-0.0.11/src/neno/models.py` & `neno-0.0.12/src/neno/models.py`

 * *Files identical despite different names*

### Comparing `neno-0.0.11/src/neno/requirements.txt` & `neno-0.0.12/src/neno/requirements.txt`

 * *Files identical despite different names*

### Comparing `neno-0.0.11/src/neno/runner.py` & `neno-0.0.12/src/neno/runner.py`

 * *Files identical despite different names*

### Comparing `neno-0.0.11/src/neno/server.py` & `neno-0.0.12/src/neno/server.py`

 * *Files identical despite different names*

### Comparing `neno-0.0.11/src/neno/storage_backends.py` & `neno-0.0.12/src/neno/storage_backends.py`

 * *Files identical despite different names*

### Comparing `neno-0.0.11/src/neno/util.py` & `neno-0.0.12/src/neno/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
   ensure_dir(venvs_dirs)
   venv_dir = _get_venv_dir(key)
   if not os.path.exists(venv_dir):
     print(f"Creating venv {venv_dir}")
     venv.create(venv_dir, with_pip=True)
     # install papermill in the venv
     print(f"venv {venv_dir} created. Installing papermill...")
-    result = subprocess.run([f"{venv_dir}/bin/pip", "install", "papermill", "ipykernel"], stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+    result = subprocess.run([f"{venv_dir}/bin/python", "-m", "pip", "install", "papermill", "ipykernel"], stdout=subprocess.PIPE, stderr=subprocess.PIPE)
     try:
       result.check_returncode()
     except subprocess.CalledProcessError as e:
       print(e.stderr.decode())
       raise e
     print(f"Installing ipykernel in {venv_dir}...")
     result = subprocess.run([f"{venv_dir}/bin/python", "-m", "ipykernel", "install", "--user"])
```

### Comparing `neno-0.0.11/src/neno/example-endpoint/test-notebook.ipynb` & `neno-0.0.12/src/neno/example-endpoint/test-notebook.ipynb`

 * *Files identical despite different names*

### Comparing `neno-0.0.11/LICENSE` & `neno-0.0.12/LICENSE`

 * *Files identical despite different names*

### Comparing `neno-0.0.11/pyproject.toml` & `neno-0.0.12/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "neno"
-version = "0.0.11"
+version = "0.0.12"
 authors = [
   { name="Alex Rovner", email="rovnero@gmail.com" },
 ]
 description = "NeNo (Network Notebooks) is a tool that allows you manage and trigger your Jupyter notebooks remotely over the network using HTTP."
 readme = "README.md"
 requires-python = ">=3.9"
 dependencies = [
```

### Comparing `neno-0.0.11/PKG-INFO` & `neno-0.0.12/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: neno
-Version: 0.0.11
+Version: 0.0.12
 Summary: NeNo (Network Notebooks) is a tool that allows you manage and trigger your Jupyter notebooks remotely over the network using HTTP.
 Project-URL: Homepage, https://github.com/snophey/nota
 Project-URL: Issues, https://github.com/snophey/nota/issues
 Author-email: Alex Rovner <rovnero@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

