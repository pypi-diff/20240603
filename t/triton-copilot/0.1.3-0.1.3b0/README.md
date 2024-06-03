# Comparing `tmp/triton_copilot-0.1.3.tar.gz` & `tmp/triton_copilot-0.1.3b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "triton_copilot-0.1.3.tar", max compression
+gzip compressed data, was "triton_copilot-0.1.3b0.tar", max compression
```

## Comparing `triton_copilot-0.1.3.tar` & `triton_copilot-0.1.3b0.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0     1635 2024-05-19 18:06:06.377881 triton_copilot-0.1.3/README.md
--rw-r--r--   0        0        0      434 2024-06-03 08:39:14.309936 triton_copilot-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-19 18:06:06.378471 triton_copilot-0.1.3/triton_copilot/__init__.py
--rw-r--r--   0        0        0     3025 2024-06-03 08:38:46.390700 triton_copilot-0.1.3/triton_copilot/build_services.py
--rw-r--r--   0        0        0    11247 2024-06-01 11:12:29.619864 triton_copilot-0.1.3/triton_copilot/constants.py
--rw-r--r--   0        0        0     1854 2024-06-01 11:18:07.099737 triton_copilot-0.1.3/triton_copilot/init_services.py
--rw-r--r--   0        0        0     6931 2024-06-03 08:38:28.594943 triton_copilot-0.1.3/triton_copilot/main.py
--rw-r--r--   0        0        0     2596 2024-06-01 14:59:11.248679 triton_copilot-0.1.3/triton_copilot/run_services.py
--rw-r--r--   0        0        0     1011 2024-05-28 18:57:41.603455 triton_copilot-0.1.3/triton_copilot/template/1/app.py
--rw-r--r--   0        0        0     9979 2024-06-01 14:59:11.249479 triton_copilot-0.1.3/triton_copilot/template/1/model.py
--rw-r--r--   0        0        0      222 2024-06-01 08:18:21.409258 triton_copilot-0.1.3/triton_copilot/template/Dockerfile
--rw-r--r--   0        0        0     6985 2024-06-03 08:23:02.677583 triton_copilot-0.1.3/triton_copilot/triton_services.py
--rw-r--r--   0        0        0     1841 2024-06-01 14:59:11.250429 triton_copilot-0.1.3/triton_copilot/utils.py
--rw-r--r--   0        0        0     4309 2024-06-03 08:23:02.677933 triton_copilot-0.1.3/triton_copilot/validate.py
--rw-r--r--   0        0        0     2267 1970-01-01 00:00:00.000000 triton_copilot-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1635 2024-05-19 18:06:06.377881 triton_copilot-0.1.3b0/README.md
+-rw-r--r--   0        0        0      439 2024-06-03 08:48:06.215176 triton_copilot-0.1.3b0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-19 18:06:06.378471 triton_copilot-0.1.3b0/triton_copilot/__init__.py
+-rw-r--r--   0        0        0     2878 2024-06-03 08:41:34.074529 triton_copilot-0.1.3b0/triton_copilot/build_services.py
+-rw-r--r--   0        0        0    11247 2024-06-01 11:12:29.619864 triton_copilot-0.1.3b0/triton_copilot/constants.py
+-rw-r--r--   0        0        0     1854 2024-06-01 11:18:07.099737 triton_copilot-0.1.3b0/triton_copilot/init_services.py
+-rw-r--r--   0        0        0     6919 2024-06-03 08:41:49.569415 triton_copilot-0.1.3b0/triton_copilot/main.py
+-rw-r--r--   0        0        0     2596 2024-06-01 14:59:11.248679 triton_copilot-0.1.3b0/triton_copilot/run_services.py
+-rw-r--r--   0        0        0     9979 2024-06-01 14:59:11.249479 triton_copilot-0.1.3b0/triton_copilot/template/1/model.py
+-rw-r--r--   0        0        0      222 2024-06-01 08:18:21.409258 triton_copilot-0.1.3b0/triton_copilot/template/Dockerfile
+-rw-r--r--   0        0        0     7596 2024-06-03 08:48:06.209093 triton_copilot-0.1.3b0/triton_copilot/triton_services.py
+-rw-r--r--   0        0        0     1841 2024-06-01 14:59:11.250429 triton_copilot-0.1.3b0/triton_copilot/utils.py
+-rw-r--r--   0        0        0     3630 2024-06-03 08:48:06.219938 triton_copilot-0.1.3b0/triton_copilot/validate.py
+-rw-r--r--   0        0        0     2269 1970-01-01 00:00:00.000000 triton_copilot-0.1.3b0/PKG-INFO
```

### Comparing `triton_copilot-0.1.3/README.md` & `triton_copilot-0.1.3b0/README.md`

 * *Files identical despite different names*

### Comparing `triton_copilot-0.1.3/triton_copilot/build_services.py` & `triton_copilot-0.1.3b0/triton_copilot/build_services.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,20 +21,16 @@
     else:
         unload_ref = typer.prompt("Enter the unload function reference [Ex: TritonClass.unload]", default="None")
 
     return load_ref, infer_ref, unload_ref
 
 
 def infer_function_refs(file_path):
-    try:
-        with open(file_path, "r") as f:
-            data = f.read()
-    except FileNotFoundError:
-        typer.secho("Error: File not found", fg=typer.colors.BRIGHT_RED)
-        raise typer.Exit()
+    with open(file_path, "r") as f:
+        data = f.read()
     tree = ast.parse(data)
     load_ref = None
     infer_ref = None
     unload_ref = None
     for node in ast.walk(tree):
         for child in ast.iter_child_nodes(node):
             child.parent = node
```

### Comparing `triton_copilot-0.1.3/triton_copilot/constants.py` & `triton_copilot-0.1.3b0/triton_copilot/constants.py`

 * *Files identical despite different names*

### Comparing `triton_copilot-0.1.3/triton_copilot/init_services.py` & `triton_copilot-0.1.3b0/triton_copilot/init_services.py`

 * *Files identical despite different names*

### Comparing `triton_copilot-0.1.3/triton_copilot/main.py` & `triton_copilot-0.1.3b0/triton_copilot/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,29 +66,29 @@
         preferred_batch_size: int = typer.Option(None, help="Preferred batch size"),
         no_prompt: bool = typer.Option(False, help="Skip prompts"),
 ):
     try:
         if not is_initialized():
             typer.secho("Please run 'triton-copilot init' to initialize the tool", fg=typer.colors.BRIGHT_RED)
             typer.Exit()
+        validate_file(file_path)
         if not no_prompt:
             if load_ref == "None":
                 load_ref, infer_ref, unload_ref = get_function_refs(file_path)
             if sample_input_file == "None":
                 sample_input_file = typer.prompt("File path of sample input payload", default="None")
             if sample_output_file == "None":
                 sample_output_file = typer.prompt("File path of sample output payload", default="None")
             if not max_batch_size:
                 batching = typer.confirm("Do you want to enable batching?")
                 max_batch_size = None
                 preferred_batch_size = None
                 if batching:
                     max_batch_size = typer.prompt("Enter the max batch size", default=2)
                     preferred_batch_size = typer.prompt("Enter the preferred batch size", default=2)
-        file_path = validate_file(file_path)
         validate_refs(load_ref, infer_ref, unload_ref, file_path)
         model = get_model()
         with Progress(
                 SpinnerColumn(),
                 TextColumn("[progress.description]{task.description}"),
                 transient=True,
         ) as progress:
```

### Comparing `triton_copilot-0.1.3/triton_copilot/run_services.py` & `triton_copilot-0.1.3b0/triton_copilot/run_services.py`

 * *Files identical despite different names*

### Comparing `triton_copilot-0.1.3/triton_copilot/template/1/model.py` & `triton_copilot-0.1.3b0/triton_copilot/template/1/model.py`

 * *Files identical despite different names*

### Comparing `triton_copilot-0.1.3/triton_copilot/triton_services.py` & `triton_copilot-0.1.3b0/triton_copilot/triton_services.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import typer
 from triton_copilot.constants import system_prompt_config_pbtxt
 from triton_copilot.init_services import get_claude_keys, get_openai_keys
 from triton_copilot.utils import copy_code_to_new_dir, claude_chat, openai_chat, get_model_name, save_config
 import pkg_resources
 import ast
+import uuid
 
 TEMPLATE_DIR = pkg_resources.resource_filename("triton_copilot", "template/")
 
 
 def get_user_prompt(file_path, sample_input, sample_output):
     with open(file_path, "r") as f:
         app_code = f.read()
@@ -126,18 +127,30 @@
     file.writelines(lines)
 
 
 def create_triton_code(file_path, load_ref, infer_ref, unload_ref):
     base_dir = os.path.dirname(file_path)
     if base_dir == "":
         base_dir = "."
-    os.makedirs("./temp", exist_ok=True)
+    os.makedirs("./temp/1", exist_ok=True)
     temp_dir = "./temp"
-    copy_code_to_new_dir(TEMPLATE_DIR, temp_dir)
     copy_code_to_new_dir(base_dir, temp_dir + "/1")
+    if file_path.split("/")[-1] == "model.py":
+        rand_id = uuid.uuid4().hex[:4]
+        new_file_path = f"{temp_dir}/1/model_{rand_id}.py"
+        os.rename(f"{temp_dir}/1/model.py", new_file_path)
+        return new_file_path
+
+    # check if there is a file called model.py in the directory
+    if "model.py" in os.listdir(os.path.dirname(temp_dir + "/1")):
+        typer.secho("Error: model.py file found in the directory, please do not use `model.py` as "
+                    "module name as it is reserved for triton entrypoint ", fg=typer.colors.BRIGHT_RED)
+        raise typer.Exit()
+
+    copy_code_to_new_dir(TEMPLATE_DIR, temp_dir)
     file = open(f"{temp_dir}/1/model.py", "r")
     lines = file.readlines()
     for i in range(len(lines)):
         lines[i] = lines[i].replace("##model_class##", load_ref.split(".")[0])
         lines[i] = lines[i].replace("##load_func##", load_ref.split(".")[1])
         lines[i] = lines[i].replace("##infer_func##", infer_ref.split(".")[1])
         if unload_ref is not None and unload_ref != "None":
```

### Comparing `triton_copilot-0.1.3/triton_copilot/utils.py` & `triton_copilot-0.1.3b0/triton_copilot/utils.py`

 * *Files identical despite different names*

### Comparing `triton_copilot-0.1.3/triton_copilot/validate.py` & `triton_copilot-0.1.3b0/triton_copilot/validate.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import ast
-import os
 import subprocess
 import typer
-import uuid
 
 
 def validate_refs(load_ref, infer_ref, unload_ref, file_path):
     if load_ref == "None" or len(load_ref.split(".")) != 2:
         typer.secho("Error: load function reference is missing or incorrect format", fg=typer.colors.BRIGHT_RED)
         raise typer.Exit()
     if infer_ref == "None" or len(infer_ref.split(".")) != 2:
@@ -90,25 +88,14 @@
 
 
 def validate_file(file_path):
     try:
         with open(file_path, "r") as f:
             data = f.read()
         ast.parse(data)
-        if file_path.split("/")[-1] == "model.py":
-            rand_id = uuid.uuid4().hex[:4]
-            new_file_path = file_path.replace("model.py", f"model_{rand_id}.py")
-            os.rename(file_path, new_file_path)
-            return new_file_path
-        # check if there is a file called model.py in the directory
-        if "model.py" in os.listdir(os.path.dirname(file_path)):
-            typer.secho("Error: model.py file found in the directory, please do not use `model.py` as "
-                        "module name as it is reserved for triton entrypoint ", fg=typer.colors.BRIGHT_RED)
-            raise typer.Exit()
-        return file_path
     except IsADirectoryError:
         typer.secho("Error: Path is a directory", fg=typer.colors.BRIGHT_RED)
         raise typer.Exit()
     except FileNotFoundError:
         typer.secho("Error: File not found", fg=typer.colors.BRIGHT_RED)
         raise typer.Exit()
     except SyntaxError as e:
```

### Comparing `triton_copilot-0.1.3/PKG-INFO` & `triton_copilot-0.1.3b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: triton-copilot
-Version: 0.1.3
+Version: 0.1.3b0
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

