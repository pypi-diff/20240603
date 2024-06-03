# Comparing `tmp/nbpretty-0.3.2.tar.gz` & `tmp/nbpretty-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbpretty-0.3.2.tar", max compression
+gzip compressed data, was "nbpretty-0.3.3.tar", max compression
```

## Comparing `nbpretty-0.3.2.tar` & `nbpretty-0.3.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1070 2024-04-11 11:28:14.012603 nbpretty-0.3.2/LICENSE
--rw-r--r--   0        0        0      167 2024-04-11 11:28:14.012603 nbpretty-0.3.2/README.rst
--rw-r--r--   0        0        0     4585 2024-04-11 11:28:14.013603 nbpretty-0.3.2/nbpretty/__init__.py
--rw-r--r--   0        0        0    10806 2024-04-11 11:28:14.013603 nbpretty-0.3.2/nbpretty/preprocessors.py
--rw-r--r--   0        0        0       33 2024-04-11 11:28:14.013603 nbpretty-0.3.2/nbpretty/templates/nbpretty/conf.json
--rw-r--r--   0        0        0     2157 2024-04-11 11:28:14.013603 nbpretty-0.3.2/nbpretty/templates/nbpretty/index.html.j2
--rw-r--r--   0        0        0     2045 2024-04-11 11:28:14.013603 nbpretty-0.3.2/nbpretty/templates/nbpretty/static/custom.css
--rw-r--r--   0        0        0     4132 2024-04-11 11:28:14.013603 nbpretty-0.3.2/nbpretty/toc.py
--rw-r--r--   0        0        0      616 2024-04-11 11:28:14.013603 nbpretty-0.3.2/nbpretty/utils.py
--rw-r--r--   0        0        0      929 2024-04-11 11:28:14.013603 nbpretty-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     1179 1970-01-01 00:00:00.000000 nbpretty-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-06-03 12:37:53.440341 nbpretty-0.3.3/LICENSE
+-rw-r--r--   0        0        0      167 2024-06-03 12:37:53.440341 nbpretty-0.3.3/README.rst
+-rw-r--r--   0        0        0     4585 2024-06-03 12:37:53.441341 nbpretty-0.3.3/nbpretty/__init__.py
+-rw-r--r--   0        0        0    10828 2024-06-03 12:37:53.441341 nbpretty-0.3.3/nbpretty/preprocessors.py
+-rw-r--r--   0        0        0       33 2024-06-03 12:37:53.441341 nbpretty-0.3.3/nbpretty/templates/nbpretty/conf.json
+-rw-r--r--   0        0        0     2157 2024-06-03 12:37:53.441341 nbpretty-0.3.3/nbpretty/templates/nbpretty/index.html.j2
+-rw-r--r--   0        0        0     2045 2024-06-03 12:37:53.441341 nbpretty-0.3.3/nbpretty/templates/nbpretty/static/custom.css
+-rw-r--r--   0        0        0     4132 2024-06-03 12:37:53.441341 nbpretty-0.3.3/nbpretty/toc.py
+-rw-r--r--   0        0        0      616 2024-06-03 12:37:53.441341 nbpretty-0.3.3/nbpretty/utils.py
+-rw-r--r--   0        0        0      951 2024-06-03 12:37:53.441341 nbpretty-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     1222 1970-01-01 00:00:00.000000 nbpretty-0.3.3/PKG-INFO
```

### Comparing `nbpretty-0.3.2/LICENSE` & `nbpretty-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nbpretty-0.3.2/nbpretty/__init__.py` & `nbpretty-0.3.3/nbpretty/__init__.py`

 * *Files identical despite different names*

### Comparing `nbpretty-0.3.2/nbpretty/preprocessors.py` & `nbpretty-0.3.3/nbpretty/preprocessors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import base64
 import hashlib
 import re
 import shlex
 from pathlib import Path
 
 from nbconvert.preprocessors import Preprocessor
+import markupsafe
 
 
 class HighlightExercises(Preprocessor):
     """
     Any cells with the tag ``exercise`` will have the ``exercise`` css class attached to them.
     By default this highlights the output cell in yellow.
     """
@@ -242,15 +243,15 @@
             env = self.parent.environment
             css_source = env.loader.get_source(env, name)[0]
             h = base64.urlsafe_b64encode(hashlib.sha1(css_source.encode()).digest()[:12]).decode()
             # static/style.css becomes, e.g. nbpretty_oNmeLFPs3BZEPiaf_style.css
             filename = Path(f"nbpretty_{h}_{Path(name).stem}.css")
             resources["files"][filename] = css_source
             code = f"""<style type="text/css">\n@import '{filename}'\n</style>"""
-            return jinja2.Markup(code)
+            return markupsafe.Markup(code)
 
         resources['import_css'] = import_css
         resources['include_css'] = import_css
 
         if "files" not in resources:
             resources["files"] = {}
         if "inlining" not in resources:
```

### Comparing `nbpretty-0.3.2/nbpretty/templates/nbpretty/index.html.j2` & `nbpretty-0.3.3/nbpretty/templates/nbpretty/index.html.j2`

 * *Files identical despite different names*

### Comparing `nbpretty-0.3.2/nbpretty/templates/nbpretty/static/custom.css` & `nbpretty-0.3.3/nbpretty/templates/nbpretty/static/custom.css`

 * *Files identical despite different names*

### Comparing `nbpretty-0.3.2/nbpretty/toc.py` & `nbpretty-0.3.3/nbpretty/toc.py`

 * *Files identical despite different names*

### Comparing `nbpretty-0.3.2/nbpretty/utils.py` & `nbpretty-0.3.3/nbpretty/utils.py`

 * *Files identical despite different names*

### Comparing `nbpretty-0.3.2/pyproject.toml` & `nbpretty-0.3.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nbpretty"
-version = "0.3.2"
+version = "0.3.3"
 description = "A tool to convert sets of Jupyter notebook files into a single, cohesive set of linked pages"
 authors = ["Matt Williams <matt@milliams.com>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://gitlab.com/milliams/nbpretty"
 documentation = "https://nbpretty.readthedocs.io"
 
@@ -16,14 +16,15 @@
 PyYAML = "^6.0"
 nbconvert = "^7.0"
 click = "^8.0"
 rich = "^13.0"
 livereload = "^2.0"
 ipython = "^8.0"
 jinja2 = "^3.1"
+markupsafe = "^2.1.5"
 
 [tool.poetry.dev-dependencies]
 pytest = "^8.0.0"
 beautifulsoup4 = "^4.0.0"
 mypy = "^1.0"
 types-PyYAML = "^6.0"
 sphinx = "^4.0.0"
```

### Comparing `nbpretty-0.3.2/PKG-INFO` & `nbpretty-0.3.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbpretty
-Version: 0.3.2
+Version: 0.3.3
 Summary: A tool to convert sets of Jupyter notebook files into a single, cohesive set of linked pages
 Home-page: https://gitlab.com/milliams/nbpretty
 License: MIT
 Author: Matt Williams
 Author-email: matt@milliams.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: click (>=8.0,<9.0)
 Requires-Dist: ipython (>=8.0,<9.0)
 Requires-Dist: jinja2 (>=3.1,<4.0)
 Requires-Dist: livereload (>=2.0,<3.0)
+Requires-Dist: markupsafe (>=2.1.5,<3.0.0)
 Requires-Dist: nbconvert (>=7.0,<8.0)
 Requires-Dist: rich (>=13.0,<14.0)
 Project-URL: Documentation, https://nbpretty.readthedocs.io
 Project-URL: Repository, https://gitlab.com/milliams/nbpretty
 Description-Content-Type: text/x-rst
 
 nbpretty
```

