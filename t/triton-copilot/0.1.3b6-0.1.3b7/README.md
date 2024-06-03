# Comparing `tmp/triton_copilot-0.1.3b6.tar.gz` & `tmp/triton_copilot-0.1.3b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "triton_copilot-0.1.3b6.tar", max compression
+gzip compressed data, was "triton_copilot-0.1.3b7.tar", max compression
```

## Comparing `triton_copilot-0.1.3b6.tar` & `triton_copilot-0.1.3b7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1635 2024-05-19 18:06:06.377881 triton_copilot-0.1.3b6/README.md
--rw-r--r--   0        0        0      436 2024-06-03 09:36:50.351128 triton_copilot-0.1.3b6/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-19 18:06:06.378471 triton_copilot-0.1.3b6/triton_copilot/__init__.py
--rw-r--r--   0        0        0     2878 2024-06-03 08:41:34.074529 triton_copilot-0.1.3b6/triton_copilot/build_services.py
--rw-r--r--   0        0        0    11247 2024-06-01 11:12:29.619864 triton_copilot-0.1.3b6/triton_copilot/constants.py
--rw-r--r--   0        0        0     1854 2024-06-01 11:18:07.099737 triton_copilot-0.1.3b6/triton_copilot/init_services.py
--rw-r--r--   0        0        0     6933 2024-06-03 09:26:12.550686 triton_copilot-0.1.3b6/triton_copilot/main.py
--rw-r--r--   0        0        0     2631 2024-06-03 09:36:30.006605 triton_copilot-0.1.3b6/triton_copilot/run_services.py
--rw-r--r--   0        0        0     9991 2024-06-03 09:21:59.859742 triton_copilot-0.1.3b6/triton_copilot/template/1/model.py
--rw-r--r--   0        0        0      222 2024-06-01 08:18:21.409258 triton_copilot-0.1.3b6/triton_copilot/template/Dockerfile
--rw-r--r--   0        0        0     7633 2024-06-03 09:23:44.263881 triton_copilot-0.1.3b6/triton_copilot/triton_services.py
--rw-r--r--   0        0        0     2335 2024-06-03 09:32:14.756610 triton_copilot-0.1.3b6/triton_copilot/utils.py
--rw-r--r--   0        0        0     3630 2024-06-03 08:48:06.219938 triton_copilot-0.1.3b6/triton_copilot/validate.py
--rw-r--r--   0        0        0     2269 1970-01-01 00:00:00.000000 triton_copilot-0.1.3b6/PKG-INFO
+-rw-r--r--   0        0        0     1635 2024-05-19 18:06:06.377881 triton_copilot-0.1.3b7/README.md
+-rw-r--r--   0        0        0      436 2024-06-03 09:40:05.278568 triton_copilot-0.1.3b7/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-19 18:06:06.378471 triton_copilot-0.1.3b7/triton_copilot/__init__.py
+-rw-r--r--   0        0        0     2878 2024-06-03 08:41:34.074529 triton_copilot-0.1.3b7/triton_copilot/build_services.py
+-rw-r--r--   0        0        0    11247 2024-06-01 11:12:29.619864 triton_copilot-0.1.3b7/triton_copilot/constants.py
+-rw-r--r--   0        0        0     1854 2024-06-01 11:18:07.099737 triton_copilot-0.1.3b7/triton_copilot/init_services.py
+-rw-r--r--   0        0        0     6944 2024-06-03 09:39:32.457911 triton_copilot-0.1.3b7/triton_copilot/main.py
+-rw-r--r--   0        0        0     2670 2024-06-03 09:39:59.733108 triton_copilot-0.1.3b7/triton_copilot/run_services.py
+-rw-r--r--   0        0        0     9991 2024-06-03 09:21:59.859742 triton_copilot-0.1.3b7/triton_copilot/template/1/model.py
+-rw-r--r--   0        0        0      222 2024-06-01 08:18:21.409258 triton_copilot-0.1.3b7/triton_copilot/template/Dockerfile
+-rw-r--r--   0        0        0     7633 2024-06-03 09:23:44.263881 triton_copilot-0.1.3b7/triton_copilot/triton_services.py
+-rw-r--r--   0        0        0     2335 2024-06-03 09:32:14.756610 triton_copilot-0.1.3b7/triton_copilot/utils.py
+-rw-r--r--   0        0        0     3630 2024-06-03 08:48:06.219938 triton_copilot-0.1.3b7/triton_copilot/validate.py
+-rw-r--r--   0        0        0     2269 1970-01-01 00:00:00.000000 triton_copilot-0.1.3b7/PKG-INFO
```

### Comparing `triton_copilot-0.1.3b6/README.md` & `triton_copilot-0.1.3b7/README.md`

 * *Files identical despite different names*

### Comparing `triton_copilot-0.1.3b6/triton_copilot/build_services.py` & `triton_copilot-0.1.3b7/triton_copilot/build_services.py`

 * *Files identical despite different names*

### Comparing `triton_copilot-0.1.3b6/triton_copilot/constants.py` & `triton_copilot-0.1.3b7/triton_copilot/constants.py`

 * *Files identical despite different names*

### Comparing `triton_copilot-0.1.3b6/triton_copilot/init_services.py` & `triton_copilot-0.1.3b7/triton_copilot/init_services.py`

 * *Files identical despite different names*

### Comparing `triton_copilot-0.1.3b6/triton_copilot/main.py` & `triton_copilot-0.1.3b7/triton_copilot/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,16 +124,16 @@
         if volume == "None":
             volume = None
         if env == "None":
             env_vars = None
         else:
             env_vars = json.loads(env)
 
-        run_docker_image(tag, volume, env_vars)
-        is_started = wait_for_container_to_start()
+        port = run_docker_image(tag, volume, env_vars)
+        is_started = wait_for_container_to_start(port)
         if is_started:
             typer.echo("Triton Inference Server is running")
             get_curl_command()
         else:
             typer.secho("Triton Inference Server failed to start in 300s, please check docker logs",
                         fg=typer.colors.BRIGHT_RED)
     except Exception as e:
```

### Comparing `triton_copilot-0.1.3b6/triton_copilot/run_services.py` & `triton_copilot-0.1.3b7/triton_copilot/run_services.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,30 +5,31 @@
 
 from triton_copilot.utils import get_free_ports
 
 
 def run_docker_image(tag, volume, env_vars):
     try:
         ports = get_free_ports()
-        command = f"docker run --rm -d --gpus all -p {ports[0]}:8000 -p {ports[1]}:8001 -p {ports[2]}:8002 "
+        command = f"docker run --rm -d --gpus all -p {ports[0]}:8000 -p {ports[1]}:8001 -p {ports[2]}:8002"
         if volume is not None:
             command = f"{command} -v {volume}"
         if env_vars:
             env_vars_str = " ".join(f"-e {key}={value}" for key, value in env_vars.items())
             command = f"{command} {env_vars_str}"
         command = f"{command} {tag}"
         subprocess.run(
             command.split(" "), stdout=subprocess.PIPE, stderr=subprocess.PIPE, check=True
         )
+        return ports[0]
     except subprocess.CalledProcessError as e:
         raise RuntimeError("command '{}' return with error (code {}): {}, error: {}".format(e.cmd, e.returncode, e.output, e.stderr))
 
 
-def wait_for_container_to_start():
-    url = "http://localhost:8000/v2/health/ready"
+def wait_for_container_to_start(port):
+    url = f"http://localhost:{port}/v2/health/ready"
     wait_time = 300
     while wait_time > 0:
         try:
             response = requests.get(url)
             if response.status_code == 200:
                 return True
             else:
@@ -37,28 +38,28 @@
         except Exception as e:
             time.sleep(10)
             wait_time -= 10
 
     return False
 
 
-def get_curl_command():
-    url = "http://localhost:8000/v2/repository/index"
+def get_curl_command(port):
+    url = f"http://localhost:{port}/v2/repository/index"
     response = requests.post(url)
     if response.status_code == 200:
         data = response.json()
         if len(data) == 0:
             typer.secho("No models found", fg=typer.colors.BRIGHT_RED)
             typer.Exit()
         for model in data:
             if model.get("state") == "READY":
                 model_name = model.get("name")
                 model_version = model.get("version")
                 typer.secho(f"Model name: {model_name}, Model version: {model_version} is ready, \n curl command to infer:")
-                typer.secho(f"curl -X POST http://localhost:8000/v2/models/{model_name}/versions/{model_version}/"
+                typer.secho(f"curl -X POST http://localhost:{port}/v2/models/{model_name}/versions/{model_version}/"
                             f"infer -H 'Content-Type: application/json' -d <payload>", fg=typer.colors.BRIGHT_GREEN)
                 typer.secho("Replace <payload> with the actual payload, refer triton docs for payload format https://github.com/triton-inference-server/server/blob/main/docs/protocol/extension_binary_data.md", fg=typer.colors.YELLOW)
             else:
                 typer.secho(f"Model {model.get('name')} is not ready", fg=typer.colors.BRIGHT_YELLOW)
     else:
         typer.secho("Failed to get model details", fg=typer.colors.BRIGHT_RED)
         typer.Exit()
```

### Comparing `triton_copilot-0.1.3b6/triton_copilot/template/1/model.py` & `triton_copilot-0.1.3b7/triton_copilot/template/1/model.py`

 * *Files identical despite different names*

### Comparing `triton_copilot-0.1.3b6/triton_copilot/triton_services.py` & `triton_copilot-0.1.3b7/triton_copilot/triton_services.py`

 * *Files identical despite different names*

### Comparing `triton_copilot-0.1.3b6/triton_copilot/utils.py` & `triton_copilot-0.1.3b7/triton_copilot/utils.py`

 * *Files identical despite different names*

### Comparing `triton_copilot-0.1.3b6/triton_copilot/validate.py` & `triton_copilot-0.1.3b7/triton_copilot/validate.py`

 * *Files identical despite different names*

### Comparing `triton_copilot-0.1.3b6/PKG-INFO` & `triton_copilot-0.1.3b7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: triton-copilot
-Version: 0.1.3b6
+Version: 0.1.3b7
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

