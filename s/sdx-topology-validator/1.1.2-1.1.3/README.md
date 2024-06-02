# Comparing `tmp/sdx_topology_validator-1.1.2.tar.gz` & `tmp/sdx_topology_validator-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdx_topology_validator-1.1.2.tar", last modified: Wed May 29 19:19:10 2024, max compression
+gzip compressed data, was "sdx_topology_validator-1.1.3.tar", last modified: Sun Jun  2 23:31:57 2024, max compression
```

## Comparing `sdx_topology_validator-1.1.2.tar` & `sdx_topology_validator-1.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 19:19:10.888756 sdx_topology_validator-1.1.2/
--rw-rw-rw-   0        0        0     2228 2024-05-29 19:19:10.887758 sdx_topology_validator-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1880 2024-05-29 19:02:04.000000 sdx_topology_validator-1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 19:19:10.844916 sdx_topology_validator-1.1.2/sdx_topology_validator/
--rw-rw-rw-   0        0        0      131 2024-05-29 11:19:32.000000 sdx_topology_validator-1.1.2/sdx_topology_validator/__init__.py
--rw-rw-rw-   0        0        0     1029 2024-05-29 19:19:05.000000 sdx_topology_validator-1.1.2/sdx_topology_validator/sdx_topology_validator.py
--rw-rw-rw-   0        0        0    12064 2024-05-22 05:12:09.000000 sdx_topology_validator-1.1.2/sdx_topology_validator/validator.yaml
-drwxrwxrwx   0        0        0        0 2024-05-29 19:19:10.886756 sdx_topology_validator-1.1.2/sdx_topology_validator.egg-info/
--rw-rw-rw-   0        0        0     2228 2024-05-29 19:19:10.000000 sdx_topology_validator-1.1.2/sdx_topology_validator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      369 2024-05-29 19:19:10.000000 sdx_topology_validator-1.1.2/sdx_topology_validator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 19:19:10.000000 sdx_topology_validator-1.1.2/sdx_topology_validator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2024-05-29 19:19:10.000000 sdx_topology_validator-1.1.2/sdx_topology_validator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2024-05-29 19:19:10.000000 sdx_topology_validator-1.1.2/sdx_topology_validator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 19:19:10.888756 sdx_topology_validator-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      586 2024-05-29 19:18:49.000000 sdx_topology_validator-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 23:31:57.334873 sdx_topology_validator-1.1.3/
+-rw-rw-rw-   0        0        0     2228 2024-06-02 23:31:57.333891 sdx_topology_validator-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1880 2024-05-29 19:02:04.000000 sdx_topology_validator-1.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 23:31:57.289028 sdx_topology_validator-1.1.3/sdx_topology_validator/
+-rw-rw-rw-   0        0        0      105 2024-06-02 23:29:26.000000 sdx_topology_validator-1.1.3/sdx_topology_validator/__init__.py
+-rw-rw-rw-   0        0        0     1203 2024-06-02 22:50:05.000000 sdx_topology_validator-1.1.3/sdx_topology_validator/topology_validator.py
+-rw-rw-rw-   0        0        0    12064 2024-05-22 05:12:09.000000 sdx_topology_validator-1.1.3/sdx_topology_validator/validator.yaml
+drwxrwxrwx   0        0        0        0 2024-06-02 23:31:57.332920 sdx_topology_validator-1.1.3/sdx_topology_validator.egg-info/
+-rw-rw-rw-   0        0        0     2228 2024-06-02 23:31:57.000000 sdx_topology_validator-1.1.3/sdx_topology_validator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      365 2024-06-02 23:31:57.000000 sdx_topology_validator-1.1.3/sdx_topology_validator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 23:31:57.000000 sdx_topology_validator-1.1.3/sdx_topology_validator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-06-02 23:31:57.000000 sdx_topology_validator-1.1.3/sdx_topology_validator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-06-02 23:31:57.000000 sdx_topology_validator-1.1.3/sdx_topology_validator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-02 23:31:57.335847 sdx_topology_validator-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      586 2024-06-02 23:31:24.000000 sdx_topology_validator-1.1.3/setup.py
```

### Comparing `sdx_topology_validator-1.1.2/PKG-INFO` & `sdx_topology_validator-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdx_topology_validator
-Version: 1.1.2
+Version: 1.1.3
 Summary: Validates the converted topology against the given OpenAPI specifications
 Author: Sai Krishna Voruganti
 Author-email: saikrishnavoruganti@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: pyyaml
 Requires-Dist: jsonref
 Requires-Dist: jsonschema
```

### Comparing `sdx_topology_validator-1.1.2/README.md` & `sdx_topology_validator-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `sdx_topology_validator-1.1.2/sdx_topology_validator/sdx_topology_validator.py` & `sdx_topology_validator-1.1.3/sdx_topology_validator/topology_validator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 import yaml
 import jsonref
 from jsonschema import validate as json_validate
 from jsonschema.exceptions import ValidationError
 import importlib.resources as pkg_resources
 
 def load_openapi_schema():
-    with pkg_resources.open_text(__name__, 'validator.yaml') as file:
+    # Adjust the package name to the actual package where the resource is located
+    package_name = 'sdx_topology_validation'
+    resource_name = 'validator.yaml'
+    
+    with pkg_resources.open_text(package_name, resource_name) as file:
         openapi_spec = yaml.safe_load(file)
     return openapi_spec
 
 def resolve_references(openapi_spec):
     return jsonref.JsonRef.replace_refs(openapi_spec)
 
 def get_validator_schema(openapi_spec):
```

### Comparing `sdx_topology_validator-1.1.2/sdx_topology_validator/validator.yaml` & `sdx_topology_validator-1.1.3/sdx_topology_validator/validator.yaml`

 * *Files identical despite different names*

### Comparing `sdx_topology_validator-1.1.2/sdx_topology_validator.egg-info/PKG-INFO` & `sdx_topology_validator-1.1.3/sdx_topology_validator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdx_topology_validator
-Version: 1.1.2
+Version: 1.1.3
 Summary: Validates the converted topology against the given OpenAPI specifications
 Author: Sai Krishna Voruganti
 Author-email: saikrishnavoruganti@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: pyyaml
 Requires-Dist: jsonref
 Requires-Dist: jsonschema
```

### Comparing `sdx_topology_validator-1.1.2/setup.py` & `sdx_topology_validator-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="sdx_topology_validator",
-    version="1.1.2",
+    version="1.1.3",
     author="Sai Krishna Voruganti",
     author_email="saikrishnavoruganti@gmail.com",
     description="Validates the converted topology against the given OpenAPI specifications",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     package_data={'sdx_topology_validator': ['validator.yaml']},
```

