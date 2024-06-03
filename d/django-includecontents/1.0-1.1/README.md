# Comparing `tmp/django_includecontents-1.0.tar.gz` & `tmp/django_includecontents-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_includecontents-1.0.tar", last modified: Thu May 16 04:23:13 2024, max compression
+gzip compressed data, was "django_includecontents-1.1.tar", last modified: Mon Jun  3 05:25:19 2024, max compression
```

## Comparing `django_includecontents-1.0.tar` & `django_includecontents-1.1.tar`

### file list

```diff
@@ -1,31 +1,32 @@
--rw-r--r--   0        0        0     8552 2024-05-16 04:18:50.873093 django_includecontents-1.0/README.md
--rw-r--r--   0        0        0        0 2024-04-09 04:42:05.196722 django_includecontents-1.0/includecontents/__init__.py
--rw-r--r--   0        0        0     1006 2024-05-16 04:16:45.636328 django_includecontents-1.0/includecontents/django/__init__.py
--rw-r--r--   0        0        0     4797 2024-05-09 01:00:11.649227 django_includecontents-1.0/includecontents/django/base.py
--rw-r--r--   0        0        0     1422 2024-05-16 04:21:18.886568 django_includecontents-1.0/includecontents/django/engine.py
--rw-r--r--   0        0        0     1662 2024-05-16 04:20:38.116526 django_includecontents-1.0/includecontents/django/loaders.py
--rw-r--r--   0        0        0        0 2024-04-09 04:42:05.196722 django_includecontents-1.0/includecontents/templatetags/__init__.py
--rw-r--r--   0        0        0    17995 2024-05-16 04:20:38.119860 django_includecontents-1.0/includecontents/templatetags/includecontents.py
--rw-r--r--   0        0        0     1236 2024-05-16 04:23:13.530027 django_includecontents-1.0/pyproject.toml
--rw-r--r--   0        0        0      149 2024-05-16 04:16:52.346333 django_includecontents-1.0/tests/settings.py
--rw-r--r--   0        0        0      163 2024-04-21 20:37:00.117665 django_includecontents-1.0/tests/templates/components/card-extend.html
--rw-r--r--   0        0        0      168 2024-05-16 04:12:52.522811 django_includecontents-1.0/tests/templates/components/card.html
--rw-r--r--   0        0        0       11 2024-05-09 01:17:58.916937 django_includecontents-1.0/tests/templates/components/context.html
--rw-r--r--   0        0        0       42 2024-04-21 22:40:07.372787 django_includecontents-1.0/tests/templates/components/empty-props.html
--rw-r--r--   0        0        0       35 2024-05-01 04:25:18.356900 django_includecontents-1.0/tests/templates/components/escape-props.html
--rw-r--r--   0        0        0        5 2024-05-02 20:42:55.088146 django_includecontents-1.0/tests/templates/components/inside/cat.html
--rw-r--r--   0        0        0       97 2024-04-21 23:11:42.498021 django_includecontents-1.0/tests/templates/components/nested-attrs.html
--rw-r--r--   0        0        0       81 2024-04-30 04:36:00.000113 django_includecontents-1.0/tests/templates/multiline.html
--rw-r--r--   0        0        0      115 2024-04-09 21:50:46.125635 django_includecontents-1.0/tests/templates/test_component/attrs.html
--rw-r--r--   0        0        0      162 2024-05-12 22:22:26.017117 django_includecontents-1.0/tests/templates/test_component/extend_class.html
--rw-r--r--   0        0        0       73 2024-04-09 21:50:46.125635 django_includecontents-1.0/tests/templates/test_component/index.html
--rw-r--r--   0        0        0       34 2024-04-09 21:51:49.385743 django_includecontents-1.0/tests/templates/test_component/missing_attr.html
--rw-r--r--   0        0        0       24 2024-04-30 04:36:02.466786 django_includecontents-1.0/tests/templates/test_component/missing_closing_tag.html
--rw-r--r--   0        0        0      118 2024-04-09 21:50:46.115635 django_includecontents-1.0/tests/templates/test_tag/basic.html
--rw-r--r--   0        0        0      123 2024-05-09 01:24:20.757096 django_includecontents-1.0/tests/templates/test_tag/basic_only.html
--rw-r--r--   0        0        0       54 2024-04-21 20:37:00.117665 django_includecontents-1.0/tests/templates/test_tag/inner.html
--rw-r--r--   0        0        0      135 2024-04-09 21:50:46.115635 django_includecontents-1.0/tests/templates/test_tag/with_attr.html
--rw-r--r--   0        0        0     4406 2024-05-16 04:20:38.116526 django_includecontents-1.0/tests/test_component.py
--rw-r--r--   0        0        0      130 2024-04-09 04:52:09.297567 django_includecontents-1.0/tests/test_multiline.py
--rw-r--r--   0        0        0     1336 2024-05-09 01:24:42.027110 django_includecontents-1.0/tests/test_tag.py
--rw-r--r--   0        0        0     9609 1970-01-01 00:00:00.000000 django_includecontents-1.0/PKG-INFO
+-rw-r--r--   0        0        0     8552 2024-06-03 05:25:05.842068 django_includecontents-1.1/README.md
+-rw-r--r--   0        0        0      231 2024-06-03 05:25:05.842068 django_includecontents-1.1/includecontents/__init__.py
+-rw-r--r--   0        0        0     1006 2024-06-03 05:25:05.842068 django_includecontents-1.1/includecontents/django/__init__.py
+-rw-r--r--   0        0        0     4797 2024-06-03 05:25:05.842068 django_includecontents-1.1/includecontents/django/base.py
+-rw-r--r--   0        0        0     1422 2024-06-03 05:25:05.842068 django_includecontents-1.1/includecontents/django/engine.py
+-rw-r--r--   0        0        0     1662 2024-06-03 05:25:05.842068 django_includecontents-1.1/includecontents/django/loaders.py
+-rw-r--r--   0        0        0     1808 2024-06-03 05:25:05.842068 django_includecontents-1.1/includecontents/next_version.py
+-rw-r--r--   0        0        0        0 2024-06-03 05:25:05.842068 django_includecontents-1.1/includecontents/templatetags/__init__.py
+-rw-r--r--   0        0        0    18068 2024-06-03 05:25:05.842068 django_includecontents-1.1/includecontents/templatetags/includecontents.py
+-rw-r--r--   0        0        0     1612 2024-06-03 05:25:19.126100 django_includecontents-1.1/pyproject.toml
+-rw-r--r--   0        0        0      149 2024-06-03 05:25:05.842068 django_includecontents-1.1/tests/settings.py
+-rw-r--r--   0        0        0      163 2024-06-03 05:25:05.842068 django_includecontents-1.1/tests/templates/components/card-extend.html
+-rw-r--r--   0        0        0      168 2024-06-03 05:25:05.842068 django_includecontents-1.1/tests/templates/components/card.html
+-rw-r--r--   0        0        0       11 2024-06-03 05:25:05.842068 django_includecontents-1.1/tests/templates/components/context.html
+-rw-r--r--   0        0        0       42 2024-06-03 05:25:05.842068 django_includecontents-1.1/tests/templates/components/empty-props.html
+-rw-r--r--   0        0        0       35 2024-06-03 05:25:05.842068 django_includecontents-1.1/tests/templates/components/escape-props.html
+-rw-r--r--   0        0        0        5 2024-06-03 05:25:05.842068 django_includecontents-1.1/tests/templates/components/inside/cat.html
+-rw-r--r--   0        0        0       97 2024-06-03 05:25:05.842068 django_includecontents-1.1/tests/templates/components/nested-attrs.html
+-rw-r--r--   0        0        0       81 2024-06-03 05:25:05.842068 django_includecontents-1.1/tests/templates/multiline.html
+-rw-r--r--   0        0        0      122 2024-06-03 05:25:05.842068 django_includecontents-1.1/tests/templates/test_component/attrs.html
+-rw-r--r--   0        0        0      162 2024-06-03 05:25:05.842068 django_includecontents-1.1/tests/templates/test_component/extend_class.html
+-rw-r--r--   0        0        0       73 2024-06-03 05:25:05.846068 django_includecontents-1.1/tests/templates/test_component/index.html
+-rw-r--r--   0        0        0       34 2024-06-03 05:25:05.846068 django_includecontents-1.1/tests/templates/test_component/missing_attr.html
+-rw-r--r--   0        0        0       24 2024-06-03 05:25:05.846068 django_includecontents-1.1/tests/templates/test_component/missing_closing_tag.html
+-rw-r--r--   0        0        0      118 2024-06-03 05:25:05.846068 django_includecontents-1.1/tests/templates/test_tag/basic.html
+-rw-r--r--   0        0        0      123 2024-06-03 05:25:05.846068 django_includecontents-1.1/tests/templates/test_tag/basic_only.html
+-rw-r--r--   0        0        0       54 2024-06-03 05:25:05.846068 django_includecontents-1.1/tests/templates/test_tag/inner.html
+-rw-r--r--   0        0        0      135 2024-06-03 05:25:05.846068 django_includecontents-1.1/tests/templates/test_tag/with_attr.html
+-rw-r--r--   0        0        0     4413 2024-06-03 05:25:05.846068 django_includecontents-1.1/tests/test_component.py
+-rw-r--r--   0        0        0      130 2024-06-03 05:25:05.846068 django_includecontents-1.1/tests/test_multiline.py
+-rw-r--r--   0        0        0     1336 2024-06-03 05:25:05.846068 django_includecontents-1.1/tests/test_tag.py
+-rw-r--r--   0        0        0     9741 1970-01-01 00:00:00.000000 django_includecontents-1.1/PKG-INFO
```

### Comparing `django_includecontents-1.0/README.md` & `django_includecontents-1.1/README.md`

 * *Files identical despite different names*

### Comparing `django_includecontents-1.0/includecontents/django/__init__.py` & `django_includecontents-1.1/includecontents/django/__init__.py`

 * *Files identical despite different names*

### Comparing `django_includecontents-1.0/includecontents/django/base.py` & `django_includecontents-1.1/includecontents/django/base.py`

 * *Files identical despite different names*

### Comparing `django_includecontents-1.0/includecontents/django/engine.py` & `django_includecontents-1.1/includecontents/django/engine.py`

 * *Files identical despite different names*

### Comparing `django_includecontents-1.0/includecontents/django/loaders.py` & `django_includecontents-1.1/includecontents/django/loaders.py`

 * *Files identical despite different names*

### Comparing `django_includecontents-1.0/includecontents/templatetags/includecontents.py` & `django_includecontents-1.1/includecontents/templatetags/includecontents.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import re
 from collections import abc
 from collections.abc import MutableMapping
 from contextlib import contextmanager
-from math import e
 from typing import Any
 
 from django import template
 from django.template import TemplateSyntaxError, Variable
 from django.template.base import FilterExpression, NodeList, Parser, TokenType
 from django.template.context import Context
 from django.template.loader_tags import construct_relative_path, do_include
@@ -80,18 +79,21 @@
         for i, bit in enumerate(bits):
             if i < 3:
                 new_bits.append(bit)
             elif match := re.match(r"(^\w+[.:][-.\w:]+)(?:=(.+))?$", bit):
                 # Nested attrs can't be handled by the standard include tag.
                 attr, value = match.groups()
                 advanced_attrs[attr] = parser.compile_filter(value or "True")
-            elif "-" in bit.split("=", 1)[0]:
+            elif "-" in bit:
                 # Attributes with a dash also can't be handled by the standard include.
-                attr, value = bit.split("=", 1)
-                advanced_attrs[attr] = parser.compile_filter(value)
+                if "=" in bit:
+                    attr, value = bit.split("=", 1)
+                else:
+                    attr, value = bit, ""
+                advanced_attrs[attr] = parser.compile_filter(value or "True")
             elif match := re.match(r"^{ *(\w+) *}$", bit):
                 # Shorthand, e.g. {attr} is equivalent to attr=attr.
                 attr = match.group(1)
                 advanced_attrs[attr] = parser.compile_filter(attr)
             else:
                 # In tag mode, attributes without a value are treated as boolean flags.
                 if "=" not in bit:
```

### Comparing `django_includecontents-1.0/pyproject.toml` & `django_includecontents-1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [project]
 name = "django-includecontents"
-version = "1.0"
 description = "Django includecontents component-like tag"
 authors = [
     { name = "Chris Beaven", email = "smileychris@gmail.com" },
 ]
+dynamic = []
 dependencies = [
     "django",
+    "packaging",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
@@ -20,34 +21,50 @@
     "Framework :: Django :: 5.0",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
+version = "1.1"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Repository = "https://github.com/SmileyChris/django-includecontents"
 
 [project.optional-dependencies]
 test = [
     "pytest",
     "pytest-django",
     "pytest-mock",
 ]
+deploy = [
+    "pdm",
+    "pdm.backend",
+]
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [tool.pdm]
 distribution = true
 
+[tool.pdm.version]
+source = "scm"
+tag_regex = "v(?P<version>[0-9]+(\\.[0-9]+)+)"
+
 [tool.pytest.ini_options]
 DJANGO_SETTINGS_MODULE = "tests.settings"
 django_find_project = false
 pythonpath = "."
+
+[tool.towncrier]
+directory = "changes"
+name = "django-includecontents"
+package = "includecontents"
+filename = "CHANGES.md"
+issue_format = "[{issue}]: https://github.com/SmileyChris/django-includecontents/issues/{issue}"
```

### Comparing `django_includecontents-1.0/tests/test_component.py` & `django_includecontents-1.1/tests/test_component.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 def test_debug_mode():
     render_to_string("test_component/index.html")
 
 
 def test_attrs():
     assert render_to_string("test_component/attrs.html") == (
         """<main>
-  <section class="mycard" id="topcard">
+  <section class="mycard" id="topcard" x-data>
   <h3 class="large">hello</h3>
   <div>
     some content
   </div>
 </section>
 </main>
 """
```

### Comparing `django_includecontents-1.0/tests/test_tag.py` & `django_includecontents-1.1/tests/test_tag.py`

 * *Files identical despite different names*

### Comparing `django_includecontents-1.0/PKG-INFO` & `django_includecontents-1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-includecontents
-Version: 1.0
+Version: 1.1
 Summary: Django includecontents component-like tag
 Author-Email: Chris Beaven <smileychris@gmail.com>
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -15,18 +15,22 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Project-URL: Repository, https://github.com/SmileyChris/django-includecontents
 Requires-Python: >=3.8
 Requires-Dist: django
+Requires-Dist: packaging
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-django; extra == "test"
 Requires-Dist: pytest-mock; extra == "test"
+Requires-Dist: pdm; extra == "deploy"
+Requires-Dist: pdm.backend; extra == "deploy"
 Provides-Extra: test
+Provides-Extra: deploy
 Description-Content-Type: text/markdown
 
 # Django IncludeContents tag
 
 Provides a component-like `{% includecontents %}` tag to Django.
 
 For example:
```

