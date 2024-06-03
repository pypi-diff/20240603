# Comparing `tmp/pkg_vers-0.0.3.tar.gz` & `tmp/pkg_vers-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkg_vers-0.0.3.tar", last modified: Sun Jun  2 15:42:35 2024, max compression
+gzip compressed data, was "pkg_vers-0.0.4.tar", last modified: Sun Jun  2 21:41:45 2024, max compression
```

## Comparing `pkg_vers-0.0.3.tar` & `pkg_vers-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 charlesfeinn   (501) staff       (20)        0 2024-06-02 15:42:35.110057 pkg_vers-0.0.3/
--rw-r--r--   0 charlesfeinn   (501) staff       (20)     1070 2024-05-25 07:57:26.000000 pkg_vers-0.0.3/LICENSE.txt
--rw-r--r--   0 charlesfeinn   (501) staff       (20)     2021 2024-06-02 15:42:35.109419 pkg_vers-0.0.3/PKG-INFO
--rw-r--r--   0 charlesfeinn   (501) staff       (20)     1529 2024-06-02 07:32:14.000000 pkg_vers-0.0.3/README.md
-drwxr-xr-x   0 charlesfeinn   (501) staff       (20)        0 2024-06-02 15:42:35.104184 pkg_vers-0.0.3/pkg_vers/
--rw-r--r--   0 charlesfeinn   (501) staff       (20)      305 2024-06-02 15:41:53.000000 pkg_vers-0.0.3/pkg_vers/__init__.py
--rw-r--r--   0 charlesfeinn   (501) staff       (20)     2928 2024-06-02 15:31:43.000000 pkg_vers-0.0.3/pkg_vers/package_manager.py
--rw-r--r--   0 charlesfeinn   (501) staff       (20)     1135 2024-06-02 15:41:08.000000 pkg_vers-0.0.3/pkg_vers/utils.py
-drwxr-xr-x   0 charlesfeinn   (501) staff       (20)        0 2024-06-02 15:42:35.108607 pkg_vers-0.0.3/pkg_vers.egg-info/
--rw-r--r--   0 charlesfeinn   (501) staff       (20)     2021 2024-06-02 15:42:35.000000 pkg_vers-0.0.3/pkg_vers.egg-info/PKG-INFO
--rw-r--r--   0 charlesfeinn   (501) staff       (20)      290 2024-06-02 15:42:35.000000 pkg_vers-0.0.3/pkg_vers.egg-info/SOURCES.txt
--rw-r--r--   0 charlesfeinn   (501) staff       (20)        1 2024-06-02 15:42:35.000000 pkg_vers-0.0.3/pkg_vers.egg-info/dependency_links.txt
--rw-r--r--   0 charlesfeinn   (501) staff       (20)        9 2024-06-02 15:42:35.000000 pkg_vers-0.0.3/pkg_vers.egg-info/top_level.txt
--rw-r--r--   0 charlesfeinn   (501) staff       (20)       94 2024-05-25 08:00:42.000000 pkg_vers-0.0.3/pyproject.toml
--rw-r--r--   0 charlesfeinn   (501) staff       (20)       38 2024-06-02 15:42:35.110207 pkg_vers-0.0.3/setup.cfg
--rw-r--r--   0 charlesfeinn   (501) staff       (20)      684 2024-06-02 15:36:48.000000 pkg_vers-0.0.3/setup.py
-drwxr-xr-x   0 charlesfeinn   (501) staff       (20)        0 2024-06-02 15:42:35.107392 pkg_vers-0.0.3/tests/
--rw-r--r--   0 charlesfeinn   (501) staff       (20)      657 2024-06-02 07:04:23.000000 pkg_vers-0.0.3/tests/test_package_manager.py
--rw-r--r--   0 charlesfeinn   (501) staff       (20)      469 2024-06-02 07:15:06.000000 pkg_vers-0.0.3/tests/test_utils.py
+drwxr-xr-x   0 charlesfeinn   (501) staff       (20)        0 2024-06-02 21:41:45.303465 pkg_vers-0.0.4/
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)     1070 2024-05-25 07:57:26.000000 pkg_vers-0.0.4/LICENSE.txt
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)     2136 2024-06-02 21:41:45.302977 pkg_vers-0.0.4/PKG-INFO
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)     1644 2024-06-02 21:40:10.000000 pkg_vers-0.0.4/README.md
+drwxr-xr-x   0 charlesfeinn   (501) staff       (20)        0 2024-06-02 21:41:45.299924 pkg_vers-0.0.4/pkg_vers/
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)      367 2024-06-02 21:35:40.000000 pkg_vers-0.0.4/pkg_vers/__init__.py
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)     4022 2024-06-02 21:41:11.000000 pkg_vers-0.0.4/pkg_vers/package_manager.py
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)     1841 2024-06-02 19:41:47.000000 pkg_vers-0.0.4/pkg_vers/utils.py
+drwxr-xr-x   0 charlesfeinn   (501) staff       (20)        0 2024-06-02 21:41:45.302507 pkg_vers-0.0.4/pkg_vers.egg-info/
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)     2136 2024-06-02 21:41:45.000000 pkg_vers-0.0.4/pkg_vers.egg-info/PKG-INFO
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)      290 2024-06-02 21:41:45.000000 pkg_vers-0.0.4/pkg_vers.egg-info/SOURCES.txt
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)        1 2024-06-02 21:41:45.000000 pkg_vers-0.0.4/pkg_vers.egg-info/dependency_links.txt
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)        9 2024-06-02 21:41:45.000000 pkg_vers-0.0.4/pkg_vers.egg-info/top_level.txt
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)       94 2024-05-25 08:00:42.000000 pkg_vers-0.0.4/pyproject.toml
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)       38 2024-06-02 21:41:45.303571 pkg_vers-0.0.4/setup.cfg
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)      684 2024-06-02 21:37:13.000000 pkg_vers-0.0.4/setup.py
+drwxr-xr-x   0 charlesfeinn   (501) staff       (20)        0 2024-06-02 21:41:45.302073 pkg_vers-0.0.4/tests/
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)      659 2024-06-02 21:34:13.000000 pkg_vers-0.0.4/tests/test_package_manager.py
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)      469 2024-06-02 07:15:06.000000 pkg_vers-0.0.4/tests/test_utils.py
```

### Comparing `pkg_vers-0.0.3/LICENSE.txt` & `pkg_vers-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pkg_vers-0.0.3/PKG-INFO` & `pkg_vers-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkg-vers
-Version: 0.0.3
+Version: 0.0.4
 Summary: pkg_vers is a utility to determine versions of top-level packages used in your project
 Home-page: https://github.com/chuckfinca/pkg_vers
 Author: Charles Feinn
 Author-email: chuckfinca@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -39,15 +39,16 @@
 ## Helper Functions
 
 For more nuanced use cases, the following helper functions are exposed:
 
 - `get_imported_top_level_packages(script_paths)`: Extract top-level imported packages from a list of script paths.
 - `get_installed_packages()`: Retrieve a dictionary of installed packages and their versions using pip and mamba.
 - `get_package_version(package)`: Get the version of a specific package using importlib.
-- `get_specific_package_versions(imported_packages, installed_packages)`: Get versions of a list of imported packages based on the installed packages.
+- `get_top_level_package_versions(imported_packages, installed_packages)`: Get versions of a list of imported packages based on the installed packages.
+- `get_package_versions_from_ipynb()`: Get versions of imported packages from an active Jupyter Notebook by name.
 
 ## Contributing
 
 Contributions are welcome! Please feel free to submit a Pull Request.
 
 ## License
```

### Comparing `pkg_vers-0.0.3/README.md` & `pkg_vers-0.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,16 @@
 ## Helper Functions
 
 For more nuanced use cases, the following helper functions are exposed:
 
 - `get_imported_top_level_packages(script_paths)`: Extract top-level imported packages from a list of script paths.
 - `get_installed_packages()`: Retrieve a dictionary of installed packages and their versions using pip and mamba.
 - `get_package_version(package)`: Get the version of a specific package using importlib.
-- `get_specific_package_versions(imported_packages, installed_packages)`: Get versions of a list of imported packages based on the installed packages.
+- `get_top_level_package_versions(imported_packages, installed_packages)`: Get versions of a list of imported packages based on the installed packages.
+- `get_package_versions_from_ipynb()`: Get versions of imported packages from an active Jupyter Notebook by name.
 
 ## Contributing
 
 Contributions are welcome! Please feel free to submit a Pull Request.
 
 ## License
```

### Comparing `pkg_vers-0.0.3/pkg_vers/package_manager.py` & `pkg_vers-0.0.4/pkg_vers/package_manager.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,65 @@
 import importlib
 import json
 import shutil
 import re
 import sys
 import ast
+import os
+import IPython
 from .utils import _run_subprocess
 
 IGNORED_LIB_MODULES = {'os', 'enum', 'random'}
 
-def extract_code_from_ipynb(notebook_path):
-    with open(notebook_path, 'r') as file:
-        notebook_content = json.load(file)
-    
-    code_cells = []
-    for cell in notebook_content['cells']:
-        if cell['cell_type'] == 'code':
-            code_cells.append(''.join(cell['source']))
+def get_imported_packages_from_ipynb():
+    try:
+        # Get the current IPython shell
+        ipython = IPython.get_ipython()
+        if ipython is None:
+            raise RuntimeError("IPython shell not found. This function must be run within a Jupyter Notebook.")
+
+        # Get all cells from the current notebook
+        cells = ipython.history_manager.input_hist_raw
+
+        # Regular expression patterns to match import statements
+        import_pattern = re.compile(r'^\s*import\s+(\S+)')
+        from_import_pattern = re.compile(r'^\s*from\s+(\S+)\s+import')
+
+        # Initialize a set to hold unique imports
+        imports = set()
+
+        # Iterate over all cells
+        for cell in cells:
+            for line in cell.split('\n'):
+                import_match = import_pattern.match(line)
+                from_import_match = from_import_pattern.match(line)
+                if import_match:
+                    imports.add(import_match.group(1).split('.')[0])
+                elif from_import_match:
+                    imports.add(from_import_match.group(1).split('.')[0])
+
+        return imports
     
-    return '\n'.join(code_cells)
+    except Exception as e:
+        print(f"An error occurred: {e}")
+        return set()
 
 def get_imported_top_level_packages(script_paths):
     imported_packages = set()
     for script_path in script_paths:
-        if script_path.endswith('.ipynb'):
-            code = extract_code_from_ipynb(script_path)
-        else:
-            with open(script_path, 'r') as file:
-                code = file.read()
+        with open(script_path, 'r') as file:
+            code = file.read()
         
-        tree = ast.parse(code, filename=script_path)
-        for node in ast.walk(tree):
-            if isinstance(node, ast.Import):
-                for alias in node.names:
-                    imported_packages.add(alias.name.split('.')[0])
-            elif isinstance(node, ast.ImportFrom):
-                imported_packages.add(node.module.split('.')[0])
+            tree = ast.parse(code, filename=script_path)
+            for node in ast.walk(tree):
+                if isinstance(node, ast.Import):
+                    for alias in node.names:
+                        imported_packages.add(alias.name.split('.')[0])
+                elif isinstance(node, ast.ImportFrom):
+                    imported_packages.add(node.module.split('.')[0])
     return list(imported_packages)
 
 def get_installed_packages():
     packages = {}
     if shutil.which('mamba'):
         mamba_lines = _run_subprocess(['mamba', 'list'])
         for line in mamba_lines:
@@ -61,15 +82,15 @@
 def get_package_version(package):
     try:
         module = importlib.import_module(package)
         return getattr(module, '__version__', '')
     except ImportError:
         return ''
 
-def get_specific_package_versions(imported_packages, installed_packages):
+def get_top_level_package_versions(imported_packages, installed_packages):
     specific_versions = {}
     for package in imported_packages:
         if package in IGNORED_LIB_MODULES:
             continue
         version = installed_packages.get(package) or installed_packages.get(package.replace("_", "-"), "")
 
         if not version:  # if version is empty, try to get it from module.__version__
@@ -79,9 +100,15 @@
 
 def get_package_versions_from(files):
     if isinstance(files, str):
         files = [files]
 
     installed_packages = get_installed_packages()
     imported_packages = get_imported_top_level_packages(files)
-    packages_with_versions = get_specific_package_versions(imported_packages, installed_packages)
+    packages_with_versions = get_top_level_package_versions(imported_packages, installed_packages)
+    return packages_with_versions
+
+def get_package_versions_from_ipynb():
+    installed_packages = get_installed_packages()
+    imported_packages = get_imported_packages_from_ipynb()
+    packages_with_versions = get_top_level_package_versions(imported_packages, installed_packages)
     return packages_with_versions
```

### Comparing `pkg_vers-0.0.3/pkg_vers.egg-info/PKG-INFO` & `pkg_vers-0.0.4/pkg_vers.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkg-vers
-Version: 0.0.3
+Version: 0.0.4
 Summary: pkg_vers is a utility to determine versions of top-level packages used in your project
 Home-page: https://github.com/chuckfinca/pkg_vers
 Author: Charles Feinn
 Author-email: chuckfinca@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -39,15 +39,16 @@
 ## Helper Functions
 
 For more nuanced use cases, the following helper functions are exposed:
 
 - `get_imported_top_level_packages(script_paths)`: Extract top-level imported packages from a list of script paths.
 - `get_installed_packages()`: Retrieve a dictionary of installed packages and their versions using pip and mamba.
 - `get_package_version(package)`: Get the version of a specific package using importlib.
-- `get_specific_package_versions(imported_packages, installed_packages)`: Get versions of a list of imported packages based on the installed packages.
+- `get_top_level_package_versions(imported_packages, installed_packages)`: Get versions of a list of imported packages based on the installed packages.
+- `get_package_versions_from_ipynb()`: Get versions of imported packages from an active Jupyter Notebook by name.
 
 ## Contributing
 
 Contributions are welcome! Please feel free to submit a Pull Request.
 
 ## License
```

### Comparing `pkg_vers-0.0.3/setup.py` & `pkg_vers-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="pkg-vers",
-    version="0.0.3",
+    version="0.0.4",
     packages=find_packages(),
     author='Charles Feinn',
     author_email='chuckfinca@gmail.com',
     description="pkg_vers is a utility to determine versions of top-level packages used in your project",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/chuckfinca/pkg_vers',
```

### Comparing `pkg_vers-0.0.3/tests/test_package_manager.py` & `pkg_vers-0.0.4/tests/test_package_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 
 class TestPackageManager(unittest.TestCase):
 
     def test_get_installed_packages(self):
         packages = pkg_vers.get_installed_packages()
         self.assertIsInstance(packages, dict)
 
-    def test_get_specific_package_versions(self):
-        versions = pkg_vers.get_specific_package_versions(['os', 'sys'], {'os': '1.0', 'sys': '2.0'})
+    def test_get_top_level_package_versions(self):
+        versions = pkg_vers.get_top_level_package_versions(['os', 'sys'], {'os': '1.0', 'sys': '2.0'})
         self.assertIsInstance(versions, dict)
 
     def test_get_imported_top_level_packages(self):
         imported_packages = pkg_vers.get_imported_top_level_packages([__file__])
         self.assertIsInstance(imported_packages, list)
 
 if __name__ == '__main__':
```

