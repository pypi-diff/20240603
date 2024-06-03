# Comparing `tmp/validate_pyproject_schema_store-2024.5.24.tar.gz` & `tmp/validate_pyproject_schema_store-2024.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Fri May 24 02:52:07 2024, max compression
+gzip compressed data, last modified: Mon Jun  3 09:10:21 2024, max compression
```

## Comparing `validate_pyproject_schema_store-2024.5.24.tar` & `validate_pyproject_schema_store-2024.6.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     2273 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/.pre-commit-config.yaml
--rw-r--r--   0        0        0      305 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/.pre-commit-hooks.yaml
--rw-r--r--   0        0        0     2412 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      224 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/.github/dependabot.yml
--rw-r--r--   0        0        0       76 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/.github/release.yml
--rw-r--r--   0        0        0      668 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/.github/matchers/pylint.json
--rw-r--r--   0        0        0     1093 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/.github/workflows/bump.yml
--rw-r--r--   0        0        0      843 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/.github/workflows/cd.yml
--rw-r--r--   0        0        0      885 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/.github/workflows/ci.yml
--rw-r--r--   0        0        0      188 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/src/validate_pyproject_schema_store/__init__.py
--rw-r--r--   0        0        0        0 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/src/validate_pyproject_schema_store/py.typed
--rw-r--r--   0        0        0     1373 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/src/validate_pyproject_schema_store/schema.py
--rw-r--r--   0        0        0     6871 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/src/validate_pyproject_schema_store/resources/black.schema.json
--rw-r--r--   0        0        0    20516 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/src/validate_pyproject_schema_store/resources/cibuildwheel.schema.json
--rw-r--r--   0        0        0    27093 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/src/validate_pyproject_schema_store/resources/hatch.schema.json
--rw-r--r--   0        0        0    44330 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/src/validate_pyproject_schema_store/resources/mypy.schema.json
--rw-r--r--   0        0        0    25354 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/src/validate_pyproject_schema_store/resources/pdm.schema.json
--rw-r--r--   0        0        0    20182 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/src/validate_pyproject_schema_store/resources/poetry.schema.json
--rw-r--r--   0        0        0    70835 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/src/validate_pyproject_schema_store/resources/pyright.schema.json
--rw-r--r--   0        0        0   128445 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/src/validate_pyproject_schema_store/resources/ruff.schema.json
--rw-r--r--   0        0        0    20535 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/src/validate_pyproject_schema_store/resources/scikit-build.schema.json
--rw-r--r--   0        0        0    13647 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/src/validate_pyproject_schema_store/resources/setuptools.schema.json
--rw-r--r--   0        0        0      691 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/src/validate_pyproject_schema_store/resources/tool.json
--rw-r--r--   0        0        0    24630 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/src/validate_pyproject_schema_store/resources/uv.schema.json
--rw-r--r--   0        0        0      890 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/tests/test_package.py
--rw-r--r--   0        0        0      850 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/tests/test_validate_pyproject.py
--rwxr-xr-x   0        0        0     2467 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/tools/sync.py
--rw-r--r--   0        0        0     2218 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/.gitignore
--rw-r--r--   0        0        0    11358 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/LICENSE
--rw-r--r--   0        0        0     2080 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/README.md
--rw-r--r--   0        0        0     4986 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/pyproject.toml
--rw-r--r--   0        0        0     4156 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/PKG-INFO
+-rw-r--r--   0        0        0     2273 2024-06-03 09:10:21.000000 validate_pyproject_schema_store-2024.6.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      305 2024-06-03 09:10:21.000000 validate_pyproject_schema_store-2024.6.3/.pre-commit-hooks.yaml
+-rw-r--r--   0        0        0     2412 2024-06-03 09:10:21.000000 validate_pyproject_schema_store-2024.6.3/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      224 2024-06-03 09:10:21.000000 validate_pyproject_schema_store-2024.6.3/.github/dependabot.yml
+-rw-r--r--   0        0        0       76 2024-06-03 09:10:21.000000 validate_pyproject_schema_store-2024.6.3/.github/release.yml
+-rw-r--r--   0        0        0      668 2024-06-03 09:10:21.000000 validate_pyproject_schema_store-2024.6.3/.github/matchers/pylint.json
+-rw-r--r--   0        0        0     1093 2024-06-03 09:10:21.000000 validate_pyproject_schema_store-2024.6.3/.github/workflows/bump.yml
+-rw-r--r--   0        0        0      843 2024-06-03 09:10:21.000000 validate_pyproject_schema_store-2024.6.3/.github/workflows/cd.yml
+-rw-r--r--   0        0        0      885 2024-06-03 09:10:21.000000 validate_pyproject_schema_store-2024.6.3/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      188 2024-06-03 09:10:21.000000 validate_pyproject_schema_store-2024.6.3/src/validate_pyproject_schema_store/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-03 09:10:21.000000 validate_pyproject_schema_store-2024.6.3/src/validate_pyproject_schema_store/py.typed
+-rw-r--r--   0        0        0     1373 2024-06-03 09:10:21.000000 validate_pyproject_schema_store-2024.6.3/src/validate_pyproject_schema_store/schema.py
+-rw-r--r--   0        0        0     6871 2024-06-03 09:10:21.000000 validate_pyproject_schema_store-2024.6.3/src/validate_pyproject_schema_store/resources/black.schema.json
+-rw-r--r--   0        0        0    20516 2024-06-03 09:10:21.000000 validate_pyproject_schema_store-2024.6.3/src/validate_pyproject_schema_store/resources/cibuildwheel.schema.json
+-rw-r--r--   0        0        0    27093 2024-06-03 09:10:21.000000 validate_pyproject_schema_store-2024.6.3/src/validate_pyproject_schema_store/resources/hatch.schema.json
+-rw-r--r--   0        0        0    44330 2024-06-03 09:10:21.000000 validate_pyproject_schema_store-2024.6.3/src/validate_pyproject_schema_store/resources/mypy.schema.json
+-rw-r--r--   0        0        0    25354 2024-06-03 09:10:21.000000 validate_pyproject_schema_store-2024.6.3/src/validate_pyproject_schema_store/resources/pdm.schema.json
+-rw-r--r--   0        0        0    20806 2024-06-03 09:10:21.000000 validate_pyproject_schema_store-2024.6.3/src/validate_pyproject_schema_store/resources/poetry.schema.json
+-rw-r--r--   0        0        0    71915 2024-06-03 09:10:21.000000 validate_pyproject_schema_store-2024.6.3/src/validate_pyproject_schema_store/resources/pyright.schema.json
+-rw-r--r--   0        0        0   128445 2024-06-03 09:10:21.000000 validate_pyproject_schema_store-2024.6.3/src/validate_pyproject_schema_store/resources/ruff.schema.json
+-rw-r--r--   0        0        0    20535 2024-06-03 09:10:21.000000 validate_pyproject_schema_store-2024.6.3/src/validate_pyproject_schema_store/resources/scikit-build.schema.json
+-rw-r--r--   0        0        0    13647 2024-06-03 09:10:21.000000 validate_pyproject_schema_store-2024.6.3/src/validate_pyproject_schema_store/resources/setuptools.schema.json
+-rw-r--r--   0        0        0      691 2024-06-03 09:10:21.000000 validate_pyproject_schema_store-2024.6.3/src/validate_pyproject_schema_store/resources/tool.json
+-rw-r--r--   0        0        0    24630 2024-06-03 09:10:21.000000 validate_pyproject_schema_store-2024.6.3/src/validate_pyproject_schema_store/resources/uv.schema.json
+-rw-r--r--   0        0        0      890 2024-06-03 09:10:21.000000 validate_pyproject_schema_store-2024.6.3/tests/test_package.py
+-rw-r--r--   0        0        0      850 2024-06-03 09:10:21.000000 validate_pyproject_schema_store-2024.6.3/tests/test_validate_pyproject.py
+-rwxr-xr-x   0        0        0     2467 2024-06-03 09:10:21.000000 validate_pyproject_schema_store-2024.6.3/tools/sync.py
+-rw-r--r--   0        0        0     2218 2024-06-03 09:10:21.000000 validate_pyproject_schema_store-2024.6.3/.gitignore
+-rw-r--r--   0        0        0    11358 2024-06-03 09:10:21.000000 validate_pyproject_schema_store-2024.6.3/LICENSE
+-rw-r--r--   0        0        0     2080 2024-06-03 09:10:21.000000 validate_pyproject_schema_store-2024.6.3/README.md
+-rw-r--r--   0        0        0     4986 2024-06-03 09:10:21.000000 validate_pyproject_schema_store-2024.6.3/pyproject.toml
+-rw-r--r--   0        0        0     4155 2024-06-03 09:10:21.000000 validate_pyproject_schema_store-2024.6.3/PKG-INFO
```

### Comparing `validate_pyproject_schema_store-2024.5.24/.pre-commit-config.yaml` & `validate_pyproject_schema_store-2024.6.3/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     hooks:
       - id: prettier
         types_or: [yaml, markdown, html, css, scss, javascript, json]
         args: [--prose-wrap=always]
         exclude: '^src/validate_pyproject_schema_store/resources/.*\.json'
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: "v0.4.4"
+    rev: "v0.4.5"
     hooks:
       - id: ruff
         args: ["--fix", "--show-fixes"]
       - id: ruff-format
 
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: "v1.10.0"
@@ -50,15 +50,15 @@
           - pytest
           - importlib_resources
           - tomlkit
           - aiohttp
           - validate_pyproject
 
   - repo: https://github.com/codespell-project/codespell
-    rev: "v2.2.6"
+    rev: "v2.3.0"
     hooks:
       - id: codespell
         args: ["-Lcrate"]
 
   - repo: https://github.com/shellcheck-py/shellcheck-py
     rev: "v0.10.0.1"
     hooks:
@@ -74,12 +74,12 @@
 
   - repo: https://github.com/abravalheri/validate-pyproject
     rev: v0.18
     hooks:
       - id: validate-pyproject
 
   - repo: https://github.com/python-jsonschema/check-jsonschema
-    rev: 0.28.3
+    rev: 0.28.4
     hooks:
       - id: check-dependabot
       - id: check-github-workflows
       - id: check-readthedocs
```

### Comparing `validate_pyproject_schema_store-2024.5.24/.github/CONTRIBUTING.md` & `validate_pyproject_schema_store-2024.6.3/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.24/.github/matchers/pylint.json` & `validate_pyproject_schema_store-2024.6.3/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.24/.github/workflows/bump.yml` & `validate_pyproject_schema_store-2024.6.3/.github/workflows/bump.yml`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.24/.github/workflows/cd.yml` & `validate_pyproject_schema_store-2024.6.3/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.24/.github/workflows/ci.yml` & `validate_pyproject_schema_store-2024.6.3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.24/src/validate_pyproject_schema_store/schema.py` & `validate_pyproject_schema_store-2024.6.3/src/validate_pyproject_schema_store/schema.py`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.24/src/validate_pyproject_schema_store/resources/black.schema.json` & `validate_pyproject_schema_store-2024.6.3/src/validate_pyproject_schema_store/resources/black.schema.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.24/src/validate_pyproject_schema_store/resources/cibuildwheel.schema.json` & `validate_pyproject_schema_store-2024.6.3/src/validate_pyproject_schema_store/resources/cibuildwheel.schema.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.24/src/validate_pyproject_schema_store/resources/hatch.schema.json` & `validate_pyproject_schema_store-2024.6.3/src/validate_pyproject_schema_store/resources/hatch.schema.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.24/src/validate_pyproject_schema_store/resources/mypy.schema.json` & `validate_pyproject_schema_store-2024.6.3/src/validate_pyproject_schema_store/resources/mypy.schema.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.24/src/validate_pyproject_schema_store/resources/pdm.schema.json` & `validate_pyproject_schema_store-2024.6.3/src/validate_pyproject_schema_store/resources/pdm.schema.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.24/src/validate_pyproject_schema_store/resources/poetry.schema.json` & `validate_pyproject_schema_store-2024.6.3/src/validate_pyproject_schema_store/resources/poetry.schema.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996744791666666%*

 * *Differences: {"'properties'": "{'plugins': {'additionalProperties': OrderedDict([('type', 'object'), "*

 * *                 "('properties', OrderedDict([('dotenv', OrderedDict([('type', 'object'), "*

 * *                 "('description', 'Configuration for the poetry-plugin-dotenv'), ('properties', "*

 * *                 "OrderedDict([('ignore', OrderedDict([('type', 'string'), ('description', 'Flag "*

 * *                 "that prevents the plugin from loading the dotenv file.')])), ('location', "*

 * *                 "OrderedDict([('type', […]*

```diff
@@ -620,14 +620,33 @@
                     "include"
                 ],
                 "type": "object"
             },
             "type": "array"
         },
         "plugins": {
+            "additionalProperties": {
+                "properties": {
+                    "dotenv": {
+                        "description": "Configuration for the poetry-plugin-dotenv",
+                        "properties": {
+                            "ignore": {
+                                "description": "Flag that prevents the plugin from loading the dotenv file.",
+                                "type": "string"
+                            },
+                            "location": {
+                                "description": "Path to the dotenv file. It can be both absolute and relative.",
+                                "type": "string"
+                            }
+                        },
+                        "type": "object"
+                    }
+                },
+                "type": "object"
+            },
             "description": "A hash of hashes representing plugins",
             "patternProperties": {
                 "^[a-zA-Z-_.0-9]+$": {
                     "patternProperties": {
                         "^[a-zA-Z-_.0-9]+$": {
                             "type": "string"
                         }
```

### Comparing `validate_pyproject_schema_store-2024.5.24/src/validate_pyproject_schema_store/resources/pyright.schema.json` & `validate_pyproject_schema_store-2024.6.3/src/validate_pyproject_schema_store/resources/pyright.schema.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9993324432576769%*

 * *Differences: {"'properties'": "{'extends': OrderedDict([('$id', '#/properties/extends'), ('type', 'string'), "*

 * *                 "('title', 'Path to configuration file that this configuration extends'), "*

 * *                 "('description', 'Path to another `.json` or `.toml` file that is used as a "*

 * *                 '"base configuration", allowing this configuration to inherit configuration '*

 * *                 'settings. Top-level keys within this configuration overwrite top-level keys in '*

 * *                 'the base confi […]*

```diff
@@ -149,14 +149,22 @@
                 ],
                 "title": "Analysis settings to use for specified subdirectories of code",
                 "type": "object"
             },
             "title": "Analysis settings to use for specified subdirectories of code",
             "type": "array"
         },
+        "extends": {
+            "$id": "#/properties/extends",
+            "description": "Path to another `.json` or `.toml` file that is used as a \"base configuration\", allowing this configuration to inherit configuration settings. Top-level keys within this configuration overwrite top-level keys in the base configuration. Multiple levels of inheritance are supported. Relative paths specified in a configuration file are resolved relative to the location of that configuration file.",
+            "pattern": "^(.*)$",
+            "title": "Path to configuration file that this configuration extends",
+            "type": "string",
+            "x-intellij-html-description": "Path to another <code>.json</code> or <code>.toml</code> file that is used as a &quot;base configuration&quot;, allowing this configuration to inherit configuration settings. Top-level keys within this configuration overwrite top-level keys in the base configuration. Multiple levels of inheritance are supported. Relative paths specified in a configuration file are resolved relative to the location of that configuration file."
+        },
         "extraPaths": {
             "$id": "#/properties/extraPaths",
             "description": "Additional search paths that will be used when searching for modules imported by files.",
             "items": {
                 "$id": "#/properties/extraPaths/items",
                 "default": "",
                 "pattern": "^(.*)$",
```

### Comparing `validate_pyproject_schema_store-2024.5.24/src/validate_pyproject_schema_store/resources/ruff.schema.json` & `validate_pyproject_schema_store-2024.6.3/src/validate_pyproject_schema_store/resources/ruff.schema.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.24/src/validate_pyproject_schema_store/resources/scikit-build.schema.json` & `validate_pyproject_schema_store-2024.6.3/src/validate_pyproject_schema_store/resources/scikit-build.schema.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.24/src/validate_pyproject_schema_store/resources/setuptools.schema.json` & `validate_pyproject_schema_store-2024.6.3/src/validate_pyproject_schema_store/resources/setuptools.schema.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.24/src/validate_pyproject_schema_store/resources/tool.json` & `validate_pyproject_schema_store-2024.6.3/src/validate_pyproject_schema_store/resources/tool.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.24/src/validate_pyproject_schema_store/resources/uv.schema.json` & `validate_pyproject_schema_store-2024.6.3/src/validate_pyproject_schema_store/resources/uv.schema.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.24/tests/test_package.py` & `validate_pyproject_schema_store-2024.6.3/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.24/tests/test_validate_pyproject.py` & `validate_pyproject_schema_store-2024.6.3/tests/test_validate_pyproject.py`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.24/tools/sync.py` & `validate_pyproject_schema_store-2024.6.3/tools/sync.py`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.24/.gitignore` & `validate_pyproject_schema_store-2024.6.3/.gitignore`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.24/LICENSE` & `validate_pyproject_schema_store-2024.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.24/README.md` & `validate_pyproject_schema_store-2024.6.3/README.md`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.24/pyproject.toml` & `validate_pyproject_schema_store-2024.6.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "validate-pyproject-schema-store"
-version = "2024.05.24"
+version = "2024.06.03"
 authors = [
   { name = "Henry Schreiner", email = "henryfs@princeton.edu" },
 ]
 description = "A plugin set for validate-pyproject and schema-store."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `validate_pyproject_schema_store-2024.5.24/PKG-INFO` & `validate_pyproject_schema_store-2024.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: validate-pyproject-schema-store
-Version: 2024.5.24
+Version: 2024.6.3
 Summary: A plugin set for validate-pyproject and schema-store.
 Project-URL: Homepage, https://github.com/henryiii/validate-pyproject-schema-store
 Project-URL: Bug Tracker, https://github.com/henryiii/validate-pyproject-schema-store/issues
 Project-URL: Discussions, https://github.com/henryiii/validate-pyproject-schema-store/discussions
 Project-URL: Changelog, https://github.com/henryiii/validate-pyproject-schema-store/releases
 Author-email: Henry Schreiner <henryfs@princeton.edu>
 License-File: LICENSE
```

