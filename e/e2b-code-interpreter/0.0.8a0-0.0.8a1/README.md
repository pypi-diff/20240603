# Comparing `tmp/e2b_code_interpreter-0.0.8a0.tar.gz` & `tmp/e2b_code_interpreter-0.0.8a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e2b_code_interpreter-0.0.8a0.tar", max compression
+gzip compressed data, was "e2b_code_interpreter-0.0.8a1.tar", max compression
```

## Comparing `e2b_code_interpreter-0.0.8a0.tar` & `e2b_code_interpreter-0.0.8a1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     2331 2024-06-03 09:31:46.125432 e2b_code_interpreter-0.0.8a0/README.md
--rw-r--r--   0        0        0      149 2024-06-03 09:31:46.125432 e2b_code_interpreter-0.0.8a0/e2b_code_interpreter/__init__.py
--rw-r--r--   0        0        0    14048 2024-06-03 09:31:46.125432 e2b_code_interpreter-0.0.8a0/e2b_code_interpreter/main.py
--rw-r--r--   0        0        0     8884 2024-06-03 09:31:46.129432 e2b_code_interpreter-0.0.8a0/e2b_code_interpreter/messaging.py
--rw-r--r--   0        0        0     7961 2024-06-03 09:31:46.129432 e2b_code_interpreter-0.0.8a0/e2b_code_interpreter/models.py
--rw-r--r--   0        0        0      768 2024-06-03 09:32:01.249514 e2b_code_interpreter-0.0.8a0/pyproject.toml
--rw-r--r--   0        0        0     3248 1970-01-01 00:00:00.000000 e2b_code_interpreter-0.0.8a0/PKG-INFO
+-rw-r--r--   0        0        0     2331 2024-06-03 09:53:52.568098 e2b_code_interpreter-0.0.8a1/README.md
+-rw-r--r--   0        0        0      149 2024-06-03 09:53:52.568098 e2b_code_interpreter-0.0.8a1/e2b_code_interpreter/__init__.py
+-rw-r--r--   0        0        0    14052 2024-06-03 09:53:52.568098 e2b_code_interpreter-0.0.8a1/e2b_code_interpreter/main.py
+-rw-r--r--   0        0        0     8884 2024-06-03 09:53:52.568098 e2b_code_interpreter-0.0.8a1/e2b_code_interpreter/messaging.py
+-rw-r--r--   0        0        0     7961 2024-06-03 09:53:52.568098 e2b_code_interpreter-0.0.8a1/e2b_code_interpreter/models.py
+-rw-r--r--   0        0        0      768 2024-06-03 09:54:07.936150 e2b_code_interpreter-0.0.8a1/pyproject.toml
+-rw-r--r--   0        0        0     3248 1970-01-01 00:00:00.000000 e2b_code_interpreter-0.0.8a1/PKG-INFO
```

### Comparing `e2b_code_interpreter-0.0.8a0/README.md` & `e2b_code_interpreter-0.0.8a1/README.md`

 * *Files identical despite different names*

### Comparing `e2b_code_interpreter-0.0.8a0/e2b_code_interpreter/main.py` & `e2b_code_interpreter-0.0.8a1/e2b_code_interpreter/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 
 class CodeInterpreter(Sandbox):
     """
     E2B code interpreter sandbox extension.
     """
 
-    template = "code-interpreter-stateful"
+    template = "code-interpreter-stateful-lab"
 
     def __init__(
         self,
         template: Optional[str] = None,
         api_key: Optional[str] = None,
         cwd: Optional[str] = None,
         env_vars: Optional[EnvVars] = None,
```

### Comparing `e2b_code_interpreter-0.0.8a0/e2b_code_interpreter/messaging.py` & `e2b_code_interpreter-0.0.8a1/e2b_code_interpreter/messaging.py`

 * *Files identical despite different names*

### Comparing `e2b_code_interpreter-0.0.8a0/e2b_code_interpreter/models.py` & `e2b_code_interpreter-0.0.8a1/e2b_code_interpreter/models.py`

 * *Files identical despite different names*

### Comparing `e2b_code_interpreter-0.0.8a0/pyproject.toml` & `e2b_code_interpreter-0.0.8a1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "e2b-code-interpreter"
-version = "0.0.8a0"
+version = "0.0.8a1"
 description = "E2B Code Interpreter - Stateful code execution"
 authors = ["e2b <hello@e2b.dev>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://e2b.dev/"
 repository = "https://github.com/e2b-dev/e2b-code-interpreter/tree/python"
 packages = [{ include = "e2b_code_interpreter" }]
```

### Comparing `e2b_code_interpreter-0.0.8a0/PKG-INFO` & `e2b_code_interpreter-0.0.8a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2b-code-interpreter
-Version: 0.0.8a0
+Version: 0.0.8a1
 Summary: E2B Code Interpreter - Stateful code execution
 Home-page: https://e2b.dev/
 License: Apache-2.0
 Author: e2b
 Author-email: hello@e2b.dev
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

