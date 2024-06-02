# Comparing `tmp/omniblack.utils-0.0.1.tar.gz` & `tmp/omniblack.utils-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omniblack.utils-0.0.1.tar", last modified: Wed May 15 23:57:18 2024, max compression
+gzip compressed data, was "omniblack.utils-0.0.2.tar", last modified: Sun Jun  2 22:04:01 2024, max compression
```

## Comparing `omniblack.utils-0.0.1.tar` & `omniblack.utils-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,22 @@
-drwxr-xr-x   0 terryp    (1000) terryp    (1000)        0 2024-05-15 23:57:18.925959 omniblack.utils-0.0.1/
--rw-r--r--   0 terryp    (1000) terryp    (1000)    11358 2023-02-07 20:02:33.000000 omniblack.utils-0.0.1/LICENSE.txt
--rw-r--r--   0 terryp    (1000) terryp    (1000)       27 2024-05-12 00:19:11.000000 omniblack.utils-0.0.1/MANIFEST.in
--rw-r--r--   0 terryp    (1000) terryp    (1000)    13260 2024-05-15 23:57:18.924959 omniblack.utils-0.0.1/PKG-INFO
--rw-r--r--   0 terryp    (1000) terryp    (1000)       43 2024-05-05 19:38:31.000000 omniblack.utils-0.0.1/package_config.yaml
--rw-r--r--   0 terryp    (1000) terryp    (1000)      520 2024-05-12 00:19:11.000000 omniblack.utils-0.0.1/pyproject.toml
--rw-r--r--   0 terryp    (1000) terryp    (1000)       38 2024-05-15 23:57:18.925959 omniblack.utils-0.0.1/setup.cfg
-drwxr-xr-x   0 terryp    (1000) terryp    (1000)        0 2024-05-15 23:57:18.921959 omniblack.utils-0.0.1/src/
-drwxr-xr-x   0 terryp    (1000) terryp    (1000)        0 2024-05-15 23:57:18.921959 omniblack.utils-0.0.1/src/omniblack/
-drwxr-xr-x   0 terryp    (1000) terryp    (1000)        0 2024-05-15 23:57:18.924959 omniblack.utils-0.0.1/src/omniblack/utils/
--rw-r--r--   0 terryp    (1000) terryp    (1000)       81 2024-05-05 19:38:31.000000 omniblack.utils-0.0.1/src/omniblack/utils/__init__.py
--rw-r--r--   0 terryp    (1000) terryp    (1000)      430 2024-05-11 00:02:20.000000 omniblack.utils-0.0.1/src/omniblack/utils/dep_resolver.py
--rw-r--r--   0 terryp    (1000) terryp    (1000)      826 2024-05-05 19:38:31.000000 omniblack.utils-0.0.1/src/omniblack/utils/enum.py
--rw-r--r--   0 terryp    (1000) terryp    (1000)     1945 2024-05-05 19:38:31.000000 omniblack.utils-0.0.1/src/omniblack/utils/export.py
--rw-r--r--   0 terryp    (1000) terryp    (1000)      572 2024-05-05 19:38:31.000000 omniblack.utils-0.0.1/src/omniblack/utils/module.py
--rw-r--r--   0 terryp    (1000) terryp    (1000)     2141 2024-05-05 19:38:31.000000 omniblack.utils-0.0.1/src/omniblack/utils/settings.py
-drwxr-xr-x   0 terryp    (1000) terryp    (1000)        0 2024-05-15 23:57:18.923959 omniblack.utils-0.0.1/src/omniblack.utils.egg-info/
--rw-r--r--   0 terryp    (1000) terryp    (1000)    13260 2024-05-15 23:57:18.000000 omniblack.utils-0.0.1/src/omniblack.utils.egg-info/PKG-INFO
--rw-r--r--   0 terryp    (1000) terryp    (1000)      522 2024-05-15 23:57:18.000000 omniblack.utils-0.0.1/src/omniblack.utils.egg-info/SOURCES.txt
--rw-r--r--   0 terryp    (1000) terryp    (1000)        1 2024-05-15 23:57:18.000000 omniblack.utils-0.0.1/src/omniblack.utils.egg-info/dependency_links.txt
--rw-r--r--   0 terryp    (1000) terryp    (1000)       49 2024-05-15 23:57:18.000000 omniblack.utils-0.0.1/src/omniblack.utils.egg-info/omniblack_package.json
--rw-r--r--   0 terryp    (1000) terryp    (1000)       43 2024-04-02 00:08:47.000000 omniblack.utils-0.0.1/src/omniblack.utils.egg-info/omniblack_package.yaml
--rw-r--r--   0 terryp    (1000) terryp    (1000)       10 2024-05-15 23:57:18.000000 omniblack.utils-0.0.1/src/omniblack.utils.egg-info/top_level.txt
+drwxr-xr-x   0 terryp    (1000) terryp    (1000)        0 2024-06-02 22:04:01.443287 omniblack.utils-0.0.2/
+-rw-r--r--   0 terryp    (1000) terryp    (1000)    11358 2023-02-07 20:02:33.000000 omniblack.utils-0.0.2/LICENSE.txt
+-rw-r--r--   0 terryp    (1000) terryp    (1000)       27 2024-05-31 22:48:12.000000 omniblack.utils-0.0.2/MANIFEST.in
+-rw-r--r--   0 terryp    (1000) terryp    (1000)    13260 2024-06-02 22:04:01.443287 omniblack.utils-0.0.2/PKG-INFO
+-rw-r--r--   0 terryp    (1000) terryp    (1000)       43 2024-05-31 22:48:12.000000 omniblack.utils-0.0.2/package_config.yaml
+-rw-r--r--   0 terryp    (1000) terryp    (1000)      520 2024-06-02 22:03:34.000000 omniblack.utils-0.0.2/pyproject.toml
+-rw-r--r--   0 terryp    (1000) terryp    (1000)       38 2024-06-02 22:04:01.443287 omniblack.utils-0.0.2/setup.cfg
+drwxr-xr-x   0 terryp    (1000) terryp    (1000)        0 2024-06-02 22:04:01.440287 omniblack.utils-0.0.2/src/
+drwxr-xr-x   0 terryp    (1000) terryp    (1000)        0 2024-06-02 22:04:01.440287 omniblack.utils-0.0.2/src/omniblack/
+drwxr-xr-x   0 terryp    (1000) terryp    (1000)        0 2024-06-02 22:04:01.442287 omniblack.utils-0.0.2/src/omniblack/utils/
+-rw-r--r--   0 terryp    (1000) terryp    (1000)       81 2024-05-31 22:48:12.000000 omniblack.utils-0.0.2/src/omniblack/utils/__init__.py
+-rw-r--r--   0 terryp    (1000) terryp    (1000)      451 2024-05-31 22:48:12.000000 omniblack.utils-0.0.2/src/omniblack/utils/dep_resolver.py
+-rw-r--r--   0 terryp    (1000) terryp    (1000)      830 2024-05-31 22:48:12.000000 omniblack.utils-0.0.2/src/omniblack/utils/enum.py
+-rw-r--r--   0 terryp    (1000) terryp    (1000)     2024 2024-05-31 22:48:12.000000 omniblack.utils-0.0.2/src/omniblack/utils/export.py
+-rw-r--r--   0 terryp    (1000) terryp    (1000)      585 2024-05-31 22:48:12.000000 omniblack.utils-0.0.2/src/omniblack/utils/module.py
+drwxr-xr-x   0 terryp    (1000) terryp    (1000)        0 2024-06-02 22:04:01.441287 omniblack.utils-0.0.2/src/omniblack.utils.egg-info/
+-rw-r--r--   0 terryp    (1000) terryp    (1000)    13260 2024-06-02 22:04:01.000000 omniblack.utils-0.0.2/src/omniblack.utils.egg-info/PKG-INFO
+-rw-r--r--   0 terryp    (1000) terryp    (1000)      490 2024-06-02 22:04:01.000000 omniblack.utils-0.0.2/src/omniblack.utils.egg-info/SOURCES.txt
+-rw-r--r--   0 terryp    (1000) terryp    (1000)        1 2024-06-02 22:04:01.000000 omniblack.utils-0.0.2/src/omniblack.utils.egg-info/dependency_links.txt
+-rw-r--r--   0 terryp    (1000) terryp    (1000)       49 2024-06-02 22:04:01.000000 omniblack.utils-0.0.2/src/omniblack.utils.egg-info/omniblack_package.json
+-rw-r--r--   0 terryp    (1000) terryp    (1000)       43 2024-04-02 00:08:47.000000 omniblack.utils-0.0.2/src/omniblack.utils.egg-info/omniblack_package.yaml
+-rw-r--r--   0 terryp    (1000) terryp    (1000)       10 2024-06-02 22:04:01.000000 omniblack.utils-0.0.2/src/omniblack.utils.egg-info/top_level.txt
```

### Comparing `omniblack.utils-0.0.1/LICENSE.txt` & `omniblack.utils-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `omniblack.utils-0.0.1/PKG-INFO` & `omniblack.utils-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omniblack.utils
-Version: 0.0.1
+Version: 0.0.2
 Author-email: Terry Patterson <Terryp@wegrok.net>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `omniblack.utils-0.0.1/pyproject.toml` & `omniblack.utils-0.0.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name='omniblack.utils'
-version='0.0.1'
+version='0.0.2'
 
 [project.license]
 id = "Apache-2.0"
 file = "LICENSE.txt"
 
 [[project.authors]]
 name = "Terry Patterson"
```

### Comparing `omniblack.utils-0.0.1/src/omniblack/utils/enum.py` & `omniblack.utils-0.0.2/src/omniblack/utils/enum.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,23 +9,23 @@
         super().__init_subclass__(*args, **kwargs)
         cls._subclasses.append(cls)
 
         for yaml in cls._yaml:
             yaml.register_class(cls)
 
     @staticmethod
-    def _generate_next_value_(name, start, count, last_values):
+    def _generate_next_value_(name, _start, _count, _last_values):
         return name
 
     @classmethod
     def to_yaml(cls, representer, node):
         return representer.represent_str(node.value)
 
     @classmethod
-    def from_yaml(cls, constructor, node):
+    def from_yaml(cls, _constructor, node):
         return cls(node.value)
 
     @classmethod
     def set_yaml(cls, yaml_instance):
         cls._yaml.append(yaml_instance)
 
         for sub_cls in cls._subclasses:
```

### Comparing `omniblack.utils-0.0.1/src/omniblack/utils/export.py` & `omniblack.utils-0.0.2/src/omniblack/utils/export.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import sys
+
 from importlib import import_module
 from importlib.metadata import entry_points
 from importlib.resources import files
 
 from public import public
 
 public(public=public)
@@ -53,19 +54,20 @@
                 continue
 
             mod = import_module(mod_path)
 
             try:
                 mod_all.extend(mod.__all__)
                 for name in mod.__all__:
+                    value = getattr(mod, name)
                     if name in module_dict and name != entry_name:
-                        print(
-                            f'Colliding name "{name}" in module "{mod_path}"',
-                            file=sys.stderr,
-                        )
-                    module_dict[name] = getattr(mod, name)
+                        msg = f'Colliding name "{name}" in module "{mod_path}"'
+                        if module_dict[name] is not value:
+                            print(msg, file=sys.stderr)
+                    else:
+                        module_dict[name] = value
             except AttributeError:
                 pass
 
         module_dict['__all__'] = tuple(mod_all)
     finally:
         del module_dict
```

### Comparing `omniblack.utils-0.0.1/src/omniblack/utils/module.py` & `omniblack.utils-0.0.2/src/omniblack/utils/module.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from public import public
 
 from .export import export
 
 
 @public
-def improve_module(__name__, ignore=None):
+def improve_module(__name__, ignore=None):  # noqa A002
     sys.modules[__name__].__class__ = OmniblackModule
     export(sys.modules[__name__].__dict__, ignore)
 
 
 @public
 class OmniblackModule(ModuleType):
     def __getattr__(self, name):
```

### Comparing `omniblack.utils-0.0.1/src/omniblack.utils.egg-info/PKG-INFO` & `omniblack.utils-0.0.2/src/omniblack.utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omniblack.utils
-Version: 0.0.1
+Version: 0.0.2
 Author-email: Terry Patterson <Terryp@wegrok.net>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

