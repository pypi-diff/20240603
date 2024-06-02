# Comparing `tmp/vysp_python-0.2.2.tar.gz` & `tmp/vysp_python-0.2.3.tar.gz`

## Comparing `vysp_python-0.2.2.tar` & `vysp_python-0.2.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vysp_python-0.2.2/tests/__init__.py
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 vysp_python-0.2.2/tests/test_client.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 vysp_python-0.2.2/vysp/__init__.py
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 vysp_python-0.2.2/vysp/client.py
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 vysp_python-0.2.2/vysp/exceptions.py
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 vysp_python-0.2.2/LICENSE
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 vysp_python-0.2.2/README.md
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 vysp_python-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 vysp_python-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vysp_python-0.2.3/tests/__init__.py
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 vysp_python-0.2.3/tests/test_client.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 vysp_python-0.2.3/vysp/__init__.py
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 vysp_python-0.2.3/vysp/client.py
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 vysp_python-0.2.3/vysp/exceptions.py
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 vysp_python-0.2.3/LICENSE
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 vysp_python-0.2.3/README.md
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 vysp_python-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 vysp_python-0.2.3/PKG-INFO
```

### Comparing `vysp_python-0.2.2/tests/test_client.py` & `vysp_python-0.2.3/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `vysp_python-0.2.2/vysp/client.py` & `vysp_python-0.2.3/vysp/client.py`

 * *Files identical despite different names*

### Comparing `vysp_python-0.2.2/vysp/exceptions.py` & `vysp_python-0.2.3/vysp/exceptions.py`

 * *Files identical despite different names*

### Comparing `vysp_python-0.2.2/LICENSE` & `vysp_python-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vysp_python-0.2.2/README.md` & `vysp_python-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `vysp_python-0.2.2/pyproject.toml` & `vysp_python-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["vysp"]
 
 [project]
 name = "vysp-python"
-version = "0.2.2"
+version = "0.2.3"
 authors = [
   { name="VSY Design LLC", email="vijeet@vsy.one" },
 ]
 description = "Python Client Library for VYSP.AI"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `vysp_python-0.2.2/PKG-INFO` & `vysp_python-0.2.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: vysp-python
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python Client Library for VYSP.AI
 Project-URL: Homepage, https://vysp.ai
 Project-URL: Documentation, https://docs.vysp.ai
 Project-URL: Issues, https://vysp.ai/support
 Author-email: VSY Design LLC <vijeet@vsy.one>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

