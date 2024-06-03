# Comparing `tmp/triton_copilot-0.1.3b5.tar.gz` & `tmp/triton_copilot-0.1.3b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "triton_copilot-0.1.3b5.tar", max compression
+gzip compressed data, was "triton_copilot-0.1.3b6.tar", max compression
```

## Comparing `triton_copilot-0.1.3b5.tar` & `triton_copilot-0.1.3b6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1635 2024-05-19 18:06:06.377881 triton_copilot-0.1.3b5/README.md
--rw-r--r--   0        0        0      436 2024-06-03 09:23:51.758021 triton_copilot-0.1.3b5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-19 18:06:06.378471 triton_copilot-0.1.3b5/triton_copilot/__init__.py
--rw-r--r--   0        0        0     2878 2024-06-03 08:41:34.074529 triton_copilot-0.1.3b5/triton_copilot/build_services.py
--rw-r--r--   0        0        0    11247 2024-06-01 11:12:29.619864 triton_copilot-0.1.3b5/triton_copilot/constants.py
--rw-r--r--   0        0        0     1854 2024-06-01 11:18:07.099737 triton_copilot-0.1.3b5/triton_copilot/init_services.py
--rw-r--r--   0        0        0     6919 2024-06-03 08:41:49.569415 triton_copilot-0.1.3b5/triton_copilot/main.py
--rw-r--r--   0        0        0     2596 2024-06-01 14:59:11.248679 triton_copilot-0.1.3b5/triton_copilot/run_services.py
--rw-r--r--   0        0        0     9991 2024-06-03 09:21:59.859742 triton_copilot-0.1.3b5/triton_copilot/template/1/model.py
--rw-r--r--   0        0        0      222 2024-06-01 08:18:21.409258 triton_copilot-0.1.3b5/triton_copilot/template/Dockerfile
--rw-r--r--   0        0        0     7633 2024-06-03 09:23:44.263881 triton_copilot-0.1.3b5/triton_copilot/triton_services.py
--rw-r--r--   0        0        0     1852 2024-06-03 09:08:34.242320 triton_copilot-0.1.3b5/triton_copilot/utils.py
--rw-r--r--   0        0        0     3630 2024-06-03 08:48:06.219938 triton_copilot-0.1.3b5/triton_copilot/validate.py
--rw-r--r--   0        0        0     2269 1970-01-01 00:00:00.000000 triton_copilot-0.1.3b5/PKG-INFO
+-rw-r--r--   0        0        0     1635 2024-05-19 18:06:06.377881 triton_copilot-0.1.3b6/README.md
+-rw-r--r--   0        0        0      436 2024-06-03 09:36:50.351128 triton_copilot-0.1.3b6/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-19 18:06:06.378471 triton_copilot-0.1.3b6/triton_copilot/__init__.py
+-rw-r--r--   0        0        0     2878 2024-06-03 08:41:34.074529 triton_copilot-0.1.3b6/triton_copilot/build_services.py
+-rw-r--r--   0        0        0    11247 2024-06-01 11:12:29.619864 triton_copilot-0.1.3b6/triton_copilot/constants.py
+-rw-r--r--   0        0        0     1854 2024-06-01 11:18:07.099737 triton_copilot-0.1.3b6/triton_copilot/init_services.py
+-rw-r--r--   0        0        0     6933 2024-06-03 09:26:12.550686 triton_copilot-0.1.3b6/triton_copilot/main.py
+-rw-r--r--   0        0        0     2631 2024-06-03 09:36:30.006605 triton_copilot-0.1.3b6/triton_copilot/run_services.py
+-rw-r--r--   0        0        0     9991 2024-06-03 09:21:59.859742 triton_copilot-0.1.3b6/triton_copilot/template/1/model.py
+-rw-r--r--   0        0        0      222 2024-06-01 08:18:21.409258 triton_copilot-0.1.3b6/triton_copilot/template/Dockerfile
+-rw-r--r--   0        0        0     7633 2024-06-03 09:23:44.263881 triton_copilot-0.1.3b6/triton_copilot/triton_services.py
+-rw-r--r--   0        0        0     2335 2024-06-03 09:32:14.756610 triton_copilot-0.1.3b6/triton_copilot/utils.py
+-rw-r--r--   0        0        0     3630 2024-06-03 08:48:06.219938 triton_copilot-0.1.3b6/triton_copilot/validate.py
+-rw-r--r--   0        0        0     2269 1970-01-01 00:00:00.000000 triton_copilot-0.1.3b6/PKG-INFO
```

### Comparing `triton_copilot-0.1.3b5/README.md` & `triton_copilot-0.1.3b6/README.md`

 * *Files identical despite different names*

### Comparing `triton_copilot-0.1.3b5/triton_copilot/build_services.py` & `triton_copilot-0.1.3b6/triton_copilot/build_services.py`

 * *Files identical despite different names*

### Comparing `triton_copilot-0.1.3b5/triton_copilot/constants.py` & `triton_copilot-0.1.3b6/triton_copilot/constants.py`

 * *Files identical despite different names*

### Comparing `triton_copilot-0.1.3b5/triton_copilot/init_services.py` & `triton_copilot-0.1.3b6/triton_copilot/init_services.py`

 * *Files identical despite different names*

### Comparing `triton_copilot-0.1.3b5/triton_copilot/main.py` & `triton_copilot-0.1.3b6/triton_copilot/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         typer.secho(f"Something went wrong: {e}", fg=typer.colors.BRIGHT_RED)
 
 
 @app.command(name="build")
 def build_triton(
         file_path: str = typer.Argument(help="Path to the python file"),
         tag: str = typer.Option(help="Docker image tag", prompt="Enter the image tag"),
-        triton_version: str = typer.Option("24.05-py3", help="Triton version", prompt="Enter the Triton version"),
+        triton_version: str = typer.Option("24.05-trtllm-python-py3", help="Triton version", prompt="Enter the Triton version"),
         load_ref: str = typer.Option(default="None", help="Reference to the load function"),
         infer_ref: str = typer.Option(default="None", help="Reference to the inference function"),
         unload_ref: str = typer.Option(default="None", help="Reference to the unload function"),
         sample_input_file: str = typer.Option("None", help="file path to sample input payload"),
         sample_output_file: str = typer.Option("None", help="file path to Sample output payload"),
         max_batch_size: int = typer.Option(None, help="Max batch size"),
         preferred_batch_size: int = typer.Option(None, help="Preferred batch size"),
```

### Comparing `triton_copilot-0.1.3b5/triton_copilot/run_services.py` & `triton_copilot-0.1.3b6/triton_copilot/run_services.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 import time
 import requests
 import typer
 import subprocess
 
+from triton_copilot.utils import get_free_ports
+
+
 def run_docker_image(tag, volume, env_vars):
     try:
-        command = f"docker run --rm -d --gpus all -p 8000:8000 -p 8001:8001 -p 8002:8002"
+        ports = get_free_ports()
+        command = f"docker run --rm -d --gpus all -p {ports[0]}:8000 -p {ports[1]}:8001 -p {ports[2]}:8002 "
         if volume is not None:
             command = f"{command} -v {volume}"
         if env_vars:
             env_vars_str = " ".join(f"-e {key}={value}" for key, value in env_vars.items())
             command = f"{command} {env_vars_str}"
         command = f"{command} {tag}"
         subprocess.run(
             command.split(" "), stdout=subprocess.PIPE, stderr=subprocess.PIPE, check=True
         )
     except subprocess.CalledProcessError as e:
         raise RuntimeError("command '{}' return with error (code {}): {}, error: {}".format(e.cmd, e.returncode, e.output, e.stderr))
-    except Exception as e:
-        raise SystemExit(f"Error: {e}")
 
 
 def wait_for_container_to_start():
     url = "http://localhost:8000/v2/health/ready"
     wait_time = 300
     while wait_time > 0:
         try:
```

### Comparing `triton_copilot-0.1.3b5/triton_copilot/template/1/model.py` & `triton_copilot-0.1.3b6/triton_copilot/template/1/model.py`

 * *Files identical despite different names*

### Comparing `triton_copilot-0.1.3b5/triton_copilot/triton_services.py` & `triton_copilot-0.1.3b6/triton_copilot/triton_services.py`

 * *Files identical despite different names*

### Comparing `triton_copilot-0.1.3b5/triton_copilot/utils.py` & `triton_copilot-0.1.3b6/triton_copilot/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-import shutil
+import socket
 
 import anthropic
 from openai import OpenAI
 import pkg_resources
 import shutil
 
 TEMPLATE_DIR = pkg_resources.resource_filename("triton_copilot", "template/")
@@ -66,7 +66,24 @@
 
 
 def cleanup(directory):
     try:
         shutil.rmtree(directory)  # Delete the directory and its contents recursively
     except FileNotFoundError:
         pass
+
+
+def get_free_ports():
+    start = 8000
+    end = 8999
+    ports = []
+    for port in range(start, end + 1):
+        with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
+            try:
+                s.bind(("localhost", port))
+                s.listen(1)
+                ports.append(port)
+            except OSError:
+                continue
+        if len(ports) == 3:
+            return ports
+    raise RuntimeError(f"No free ports found in the range {start}-{end}")
```

### Comparing `triton_copilot-0.1.3b5/triton_copilot/validate.py` & `triton_copilot-0.1.3b6/triton_copilot/validate.py`

 * *Files identical despite different names*

### Comparing `triton_copilot-0.1.3b5/PKG-INFO` & `triton_copilot-0.1.3b6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: triton-copilot
-Version: 0.1.3b5
+Version: 0.1.3b6
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

