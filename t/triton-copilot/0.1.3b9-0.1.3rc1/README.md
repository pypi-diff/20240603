# Comparing `tmp/triton_copilot-0.1.3b9.tar.gz` & `tmp/triton_copilot-0.1.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "triton_copilot-0.1.3b9.tar", max compression
+gzip compressed data, was "triton_copilot-0.1.3rc1.tar", max compression
```

## Comparing `triton_copilot-0.1.3b9.tar` & `triton_copilot-0.1.3rc1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1635 2024-05-19 18:06:06.377881 triton_copilot-0.1.3b9/README.md
--rw-r--r--   0        0        0      436 2024-06-03 14:02:20.939925 triton_copilot-0.1.3b9/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-19 18:06:06.378471 triton_copilot-0.1.3b9/triton_copilot/__init__.py
--rw-r--r--   0        0        0     2878 2024-06-03 08:41:34.074529 triton_copilot-0.1.3b9/triton_copilot/build_services.py
--rw-r--r--   0        0        0    11247 2024-06-01 11:12:29.619864 triton_copilot-0.1.3b9/triton_copilot/constants.py
--rw-r--r--   0        0        0     1854 2024-06-01 11:18:07.099737 triton_copilot-0.1.3b9/triton_copilot/init_services.py
--rw-r--r--   0        0        0     7465 2024-06-03 09:43:20.382370 triton_copilot-0.1.3b9/triton_copilot/main.py
--rw-r--r--   0        0        0     3107 2024-06-03 14:02:07.748266 triton_copilot-0.1.3b9/triton_copilot/run_services.py
--rw-r--r--   0        0        0     9991 2024-06-03 09:21:59.859742 triton_copilot-0.1.3b9/triton_copilot/template/1/model.py
--rw-r--r--   0        0        0      222 2024-06-01 08:18:21.409258 triton_copilot-0.1.3b9/triton_copilot/template/Dockerfile
--rw-r--r--   0        0        0     7633 2024-06-03 09:23:44.263881 triton_copilot-0.1.3b9/triton_copilot/triton_services.py
--rw-r--r--   0        0        0     2511 2024-06-03 09:54:42.607866 triton_copilot-0.1.3b9/triton_copilot/utils.py
--rw-r--r--   0        0        0     3630 2024-06-03 08:48:06.219938 triton_copilot-0.1.3b9/triton_copilot/validate.py
--rw-r--r--   0        0        0     2269 1970-01-01 00:00:00.000000 triton_copilot-0.1.3b9/PKG-INFO
+-rw-r--r--   0        0        0     1635 2024-05-19 18:06:06.377881 triton_copilot-0.1.3rc1/README.md
+-rw-r--r--   0        0        0      436 2024-06-03 14:09:49.702016 triton_copilot-0.1.3rc1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-19 18:06:06.378471 triton_copilot-0.1.3rc1/triton_copilot/__init__.py
+-rw-r--r--   0        0        0     2878 2024-06-03 08:41:34.074529 triton_copilot-0.1.3rc1/triton_copilot/build_services.py
+-rw-r--r--   0        0        0    11247 2024-06-01 11:12:29.619864 triton_copilot-0.1.3rc1/triton_copilot/constants.py
+-rw-r--r--   0        0        0     1854 2024-06-01 11:18:07.099737 triton_copilot-0.1.3rc1/triton_copilot/init_services.py
+-rw-r--r--   0        0        0     7465 2024-06-03 09:43:20.382370 triton_copilot-0.1.3rc1/triton_copilot/main.py
+-rw-r--r--   0        0        0     3082 2024-06-03 14:09:33.492665 triton_copilot-0.1.3rc1/triton_copilot/run_services.py
+-rw-r--r--   0        0        0     9991 2024-06-03 09:21:59.859742 triton_copilot-0.1.3rc1/triton_copilot/template/1/model.py
+-rw-r--r--   0        0        0      222 2024-06-01 08:18:21.409258 triton_copilot-0.1.3rc1/triton_copilot/template/Dockerfile
+-rw-r--r--   0        0        0     7633 2024-06-03 09:23:44.263881 triton_copilot-0.1.3rc1/triton_copilot/triton_services.py
+-rw-r--r--   0        0        0     2511 2024-06-03 09:54:42.607866 triton_copilot-0.1.3rc1/triton_copilot/utils.py
+-rw-r--r--   0        0        0     3630 2024-06-03 08:48:06.219938 triton_copilot-0.1.3rc1/triton_copilot/validate.py
+-rw-r--r--   0        0        0     2270 1970-01-01 00:00:00.000000 triton_copilot-0.1.3rc1/PKG-INFO
```

### Comparing `triton_copilot-0.1.3b9/README.md` & `triton_copilot-0.1.3rc1/README.md`

 * *Files identical despite different names*

### Comparing `triton_copilot-0.1.3b9/triton_copilot/build_services.py` & `triton_copilot-0.1.3rc1/triton_copilot/build_services.py`

 * *Files identical despite different names*

### Comparing `triton_copilot-0.1.3b9/triton_copilot/constants.py` & `triton_copilot-0.1.3rc1/triton_copilot/constants.py`

 * *Files identical despite different names*

### Comparing `triton_copilot-0.1.3b9/triton_copilot/init_services.py` & `triton_copilot-0.1.3rc1/triton_copilot/init_services.py`

 * *Files identical despite different names*

### Comparing `triton_copilot-0.1.3b9/triton_copilot/main.py` & `triton_copilot-0.1.3rc1/triton_copilot/main.py`

 * *Files identical despite different names*

### Comparing `triton_copilot-0.1.3b9/triton_copilot/run_services.py` & `triton_copilot-0.1.3rc1/triton_copilot/run_services.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,18 +20,18 @@
             command.split(" "), stdout=subprocess.PIPE, stderr=subprocess.PIPE, check=True
         )
         build_output_lines = completed_process.stderr.decode().split('\n')
         time.sleep(10)
         if is_container_running(tag):
             return ports[0]
         else:
-            typer.secho("Failed to start Triton Inference Server, Build logs:", fg=typer.colors.BRIGHT_RED)
+            typer.secho("\nFailed to start Triton Inference Server, Build logs:\n", fg=typer.colors.BRIGHT_RED)
             for line in build_output_lines:
-                typer.secho(line, fg=typer.colors.BRIGHT_WHITE)
-            typer.Exit()
+                typer.secho(line)
+            typer.Abort()
     except subprocess.CalledProcessError as e:
         raise RuntimeError("command '{}' return with error (code {}): {}, error: {}".format(e.cmd, e.returncode, e.output, e.stderr))
 
 
 def wait_for_container_to_start(port):
     url = f"http://localhost:{port}/v2/health/ready"
     wait_time = 300
```

### Comparing `triton_copilot-0.1.3b9/triton_copilot/template/1/model.py` & `triton_copilot-0.1.3rc1/triton_copilot/template/1/model.py`

 * *Files identical despite different names*

### Comparing `triton_copilot-0.1.3b9/triton_copilot/triton_services.py` & `triton_copilot-0.1.3rc1/triton_copilot/triton_services.py`

 * *Files identical despite different names*

### Comparing `triton_copilot-0.1.3b9/triton_copilot/utils.py` & `triton_copilot-0.1.3rc1/triton_copilot/utils.py`

 * *Files identical despite different names*

### Comparing `triton_copilot-0.1.3b9/triton_copilot/validate.py` & `triton_copilot-0.1.3rc1/triton_copilot/validate.py`

 * *Files identical despite different names*

### Comparing `triton_copilot-0.1.3b9/PKG-INFO` & `triton_copilot-0.1.3rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: triton-copilot
-Version: 0.1.3b9
+Version: 0.1.3rc1
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

